Pour faire de l'ILM propre pour les Beats, il faut configurer 3 parties distinctes :
  - Le *Beats en lui même 
  - L'ILM 
  - Le template pour lier l'index et l'ILM
  
 Un exemple de configuration pour le Beats serait : 
 
 ```
setup.ilm.enabled: true
setup.ilm.rollover_alias: "auditbeat-7.3"
setup.ilm.pattern: "{now/M{yyyy.MM}}-000001"
setup.ilm.policy_name: "auditbeat-%{[agent.version]}"
```

Warning : Le nom donné sur la partie ILM (setup.ilm.rollover_alias) va prendre le dessus sur le nom de l'index configuré dans l'output 

Pour l'ILM, il est possible d'utiliser la GUI de Kibana 

La partie template n'est pas disponible dans la GUI à version du 7.3.2 il faut donc la faire en API : 

 ```
PUT _template/auditbeat-7.3.2
{
  "index_patterns": ["auditbeat-7.3.2-*"], 
  "settings": {
    "number_of_shards": 1,
    "number_of_replicas": 1,
    "index.lifecycle.name": "auditbeat-7.3.2", 
    "index.lifecycle.rollover_alias": "auditbeat-7.3.2" 
  }
}
 ```


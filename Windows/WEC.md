# COnfiguration and tips related to WEC

## The goal
Send all Windows related logs to the same server and then ingest it in your log management solution 

### How 
Activate an Subscirption by going to the Event Collector and then click on Subcription.

Add whatever parameter you want [(tips)](https://github.com/palantir/windows-event-forwarding)

If you have a lot of logs don't forget to provide a bigger space for the Event Fowarded Log File. 

### Tips and tricks 

You can do all of the above with the [WecUtil tool](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/wecutil) 

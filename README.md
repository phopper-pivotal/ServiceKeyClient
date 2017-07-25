# ServiceKeyClient
Service Keys can be used to generate credentials for a service instance running on PCF. The credentials can be made available for use by a local client, or from an app that is not deployed to PCF.
## Create Service Key
To generate credentials for a service instance, one can create service keys.
```
$ cf create-service-key MY-SERVICE MY-KEY
```
## List Service Keys
```
$ cf service-keys MY-SERVICE
```

## Get Credentials for a Service Key
```
$ cf service-key MY-SERVICE MY-KEY
```

## Delete Service Keys
```
$ cf delete-service-key MY-SERVICE MY-KEY
```

add `-f` option to force deletion without confirmation

*_Note:_* to delete a service instance any (or all) associated service keys must be deleted prior to deletion of the service instance.

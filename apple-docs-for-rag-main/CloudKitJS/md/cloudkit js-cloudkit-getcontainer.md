

- CloudKit JS
- CloudKit
-  getContainer 

Instance Method

# getContainer

Returns the container with the specified container ID.

CloudKit JS 1.0+

``` source
CloudKit.Container getContainer(
 String containerIdentifier
);
```

## Parameters 

`containerIdentifier`  

The identifier for the container you want to get.

## Return Value

The container with the specified container ID if it exists; otherwise, the value is undefined.

## See Also

### Accessing Containers

getDefaultContainer

Returns the default container.

getAllContainers

Returns all the containers that were configured.


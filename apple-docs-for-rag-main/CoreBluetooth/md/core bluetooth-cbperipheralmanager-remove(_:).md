

- Core Bluetooth
- CBPeripheralManager
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes a specified published service from the local GATT database.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remove(_ service: CBMutableService)
```

## Parameters 

`service`  

The service you want to remove.

## Discussion

Because apps on the local peripheral device share the GATT database, more than one instance of a service may exist in the database. As a result, this method removes only the instance of the service that your app added to the database (using the add(_:) method). If any other services contains this service, you must first remove them.

## See Also

### Adding and Removing Services

func add(CBMutableService)

Publishes a service and any of its associated characteristics and characteristic descriptors to the local GATT database.

func removeAllServices()

Removes all published services from the local GATT database.


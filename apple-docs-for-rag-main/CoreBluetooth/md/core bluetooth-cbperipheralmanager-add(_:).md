

- Core Bluetooth
- CBPeripheralManager
-  add(\_:) 

Instance Method

# add(\_:)

Publishes a service and any of its associated characteristics and characteristic descriptors to the local GATT database.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func add(_ service: CBMutableService)
```

## Parameters 

`service`  

The service you want to publish.

## Discussion

When you add a service to the database, the peripheral manager calls the peripheralManager(_:didAdd:error:) method of its delegate object. If the service contains any included services, you must first publish them.

## See Also

### Adding and Removing Services

func remove(CBMutableService)

Removes a specified published service from the local GATT database.

func removeAllServices()

Removes all published services from the local GATT database.


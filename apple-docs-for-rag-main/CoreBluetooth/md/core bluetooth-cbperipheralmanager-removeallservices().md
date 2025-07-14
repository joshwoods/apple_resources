

- Core Bluetooth
- CBPeripheralManager
-  removeAllServices() 

Instance Method

# removeAllServices()

Removes all published services from the local GATT database.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeAllServices()
```

## Discussion

Use this when you want to remove all services you’ve previously published, for example, if your app has a toggle button to expose GATT services.

Because apps on the local peripheral device share the GATT database, this method removes only the services that you added using the add(_:) method. This call doesn’t remove any services published by other apps on the local peripheral device.

## See Also

### Adding and Removing Services

func add(CBMutableService)

Publishes a service and any of its associated characteristics and characteristic descriptors to the local GATT database.

func remove(CBMutableService)

Removes a specified published service from the local GATT database.


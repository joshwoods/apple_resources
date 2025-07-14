

- Core Bluetooth
- CBPeripheral
-  discoverServices(\_:) 

Instance Method

# discoverServices(\_:)

Discovers the specified services of the peripheral.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func discoverServices(_ serviceUUIDs: [CBUUID]?)
```

## Parameters 

`serviceUUIDs`  

An array of CBUUID objects that you are interested in. Each CBUUID object represents a UUID that identifies the type of service you want to discover.

## Discussion

You can provide an array of CBUUID objects—representing service UUIDs—in the `serviceUUIDs` parameter. When you do, the peripheral returns only the services of the peripheral that match the provided UUIDs.

Note

If the `servicesUUIDs` parameter is `nil`, this method returns all of the peripheral’s available services. This is much slower than providing an array of service UUIDs to search for.

When the peripheral discovers one or more services, it calls the peripheral(_:didDiscoverServices:): method of its delegate object. After a peripheral discovers services, you can access them through the peripheral’s services property.

## See Also

### Discovering Services

func discoverIncludedServices([CBUUID]?, for: CBService)

Discovers the specified included services of a previously-discovered service.

var services: [CBService]?

A list of a peripheral’s discovered services.


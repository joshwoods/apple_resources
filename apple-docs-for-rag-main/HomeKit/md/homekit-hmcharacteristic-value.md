

- HomeKit
- HMCharacteristic
-  value 

Instance Property

# value

The current value of the characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var value: Any? { get }
```

## Discussion

This is the last value that the system saw for the characteristic. Because multiple apps can access a given home, this value may change without your app changing it. To be sure you have the current value, call readValue(completionHandler:) and wait for the response before checking the value property.

You can also learn about external changes to the value when they happen by adopting the HMAccessoryDelegate protocol. Call the enableNotification(_:completionHandler:) method to enable updates for a particular characteristic. Then implement the accessory(_:service:didUpdateValueFor:) method to receive the updates. You only receive updates for changes made outside your app, for example by Apple’s Home app, or by the accessory itself.

How you interpret the value depends on the characteristicType. From this, you can tell what the value represents, and infer whether the value contain a string, integer, floating point number, or Boolean. The characteristic’s metadata gives you additional information about how to interpret and present the value.

## See Also

### Controlling a characteristic

func readValue(completionHandler: ((any Error)?) -> Void)

Reads the value for the characteristic.

func writeValue(Any?, completionHandler: ((any Error)?) -> Void)

Modifies the value of the characteristic.

func updateAuthorizationData(Data?, completionHandler: ((any Error)?) -> Void)

Sets or clears authorization data used when writing to the characteristic.




- Core Bluetooth
- CBPeripheralManager
-  isAdvertising 

Instance Property

# isAdvertising

A Boolean value that indicates whether the peripheral is advertising data.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isAdvertising: Bool { get }
```

## Discussion

This value is true if the peripheral is advertising data as a result of successfully calling the startAdvertising(_:) method. The value is false if the peripheral is no longer advertising its data.

## See Also

### Managing Advertising

func startAdvertising([String : Any]?)

Advertises peripheral manager data.

Advertising Data

func stopAdvertising()

Stops advertising peripheral manager data.


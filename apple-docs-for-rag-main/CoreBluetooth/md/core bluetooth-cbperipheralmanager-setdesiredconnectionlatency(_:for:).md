

- Core Bluetooth
- CBPeripheralManager
-  setDesiredConnectionLatency(\_:for:) 

Instance Method

# setDesiredConnectionLatency(\_:for:)

Sets the desired connection latency for an existing connection to a central device.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setDesiredConnectionLatency(
    _ latency: CBPeripheralManagerConnectionLatency,
    for central: CBCentral
)
```

## Parameters 

`latency`  

The desired connection latency. For a list of the possible connection latency values that you may set for the peripheral manager, see CBPeripheralManagerConnectionLatency.

`central`  

The central to which the peripheral manager is currently connected.

## Discussion

The latency of a peripheral-central connection controls how frequently the peripheral and the peripheral’s connected central can exchange messages. By setting a desired connection latency, you manage the relationship between the frequency of the data exchange and the resulting battery performance of the peripheral device. When you call this method to set the connection latency, note that connection latency changes aren’t guaranteed. As a result, the latency may vary. If you don’t explicitly set a latency, the central device uses the connection latency it chose when establishing the connection. Typically, you don’t need to change the connection latency.

## See Also

### Setting Connection Latency

enum CBPeripheralManagerConnectionLatency

Values representing the connection latency of the peripheral manager.


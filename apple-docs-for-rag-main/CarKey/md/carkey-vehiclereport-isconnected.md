

- CarKey
- VehicleReport
-  isConnected 

Instance Property

# isConnected

A Boolean value that indicates whether the vehicle is currently connected over Bluetooth.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.3+watchOS 9.0+

``` source
var isConnected: Bool { get }
```

## Discussion

The value of this property is `true` when the vehicle is connected over Bluetooth, or `false` when it isn’t connected.

## See Also

### Getting the Vehicle Details

let identifier: String

The string you use to identify the vehicle when making requests.


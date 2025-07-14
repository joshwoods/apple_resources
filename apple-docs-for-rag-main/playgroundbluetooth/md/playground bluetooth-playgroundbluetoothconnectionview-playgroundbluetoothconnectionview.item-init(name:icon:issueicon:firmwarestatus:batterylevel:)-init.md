

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
- PlaygroundBluetoothConnectionView.Item
-  init(name:icon:issueIcon:firmwareStatus:batteryLevel:) 

Initializer

# init(name:icon:issueIcon:firmwareStatus:batteryLevel:)

Creates a structure that holds information about a peripheral displayed in a connection view.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
init(
    name: String,
    icon: UIImage,
    issueIcon: UIImage,
    firmwareStatus: PlaygroundBluetoothConnectionView.Item.FirmwareStatus? = nil,
    batteryLevel: Double? = nil
)
```

## Parameters 

`name`  

The name of a peripheral as it should appear in a connection view.

`icon`  

An image that represents a peripheral.

`issueIcon`  

An icon indicating that a peripheral may not function correctly.

`firmwareStatus`  

A value that indicates whether a peripheral needs a firmware update.

`batteryLevel`  

A value between 0 and 1.0 indicating a peripheral’s percent battery charge.

## See Also

### Displaying Peripheral Information

var name: String

The name of a peripheral as it should appear in a connection view.


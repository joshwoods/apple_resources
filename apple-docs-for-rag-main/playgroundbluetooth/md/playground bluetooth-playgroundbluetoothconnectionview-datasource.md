

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  dataSource 

Instance Property

# dataSource

A data source that provides subviews for available peripherals.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
weak var dataSource: PlaygroundBluetoothConnectionViewDataSource?
```

## See Also

### Creating Connection Views

init(centralManager: PlaygroundBluetoothCentralManager, delegate: PlaygroundBluetoothConnectionViewDelegate?, dataSource: PlaygroundBluetoothConnectionViewDataSource?)

Creates a new, empty view that can be populated with items when peripherals are connected to the central manager.

init?(coder: NSCoder)

Creates a connection view initialized from data you supply.


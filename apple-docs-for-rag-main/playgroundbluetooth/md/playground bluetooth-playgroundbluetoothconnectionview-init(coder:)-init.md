

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  init(coder:) 

Initializer

# init(coder:)

Creates a connection view initialized from data you supply.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
required init?(coder aDecoder: NSCoder)
```

## Parameters 

`coder`  

An archive containing data that can be used to create a connection view.

## See Also

### Creating Connection Views

init(centralManager: PlaygroundBluetoothCentralManager, delegate: PlaygroundBluetoothConnectionViewDelegate?, dataSource: PlaygroundBluetoothConnectionViewDataSource?)

Creates a new, empty view that can be populated with items when peripherals are connected to the central manager.

var dataSource: PlaygroundBluetoothConnectionViewDataSource?

A data source that provides subviews for available peripherals.


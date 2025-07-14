

- Playground Bluetooth
- PlaygroundBluetoothConnectionView
-  init(centralManager:delegate:dataSource:) 

Initializer

# init(centralManager:delegate:dataSource:)

Creates a new, empty view that can be populated with items when peripherals are connected to the central manager.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
init(
    centralManager: PlaygroundBluetoothCentralManager,
    delegate: PlaygroundBluetoothConnectionViewDelegate? = nil,
    dataSource: PlaygroundBluetoothConnectionViewDataSource? = nil
)
```

## Parameters 

`centralManager`  

The central manager whose peripherals will be displayed in the view.

`delegate`  

A delegate you supply to make decisions about which peripherals are displayed in the view.

`dataSource`  

A data source that provides subviews for available peripherals.

## See Also

### Creating Connection Views

init?(coder: NSCoder)

Creates a connection view initialized from data you supply.

var dataSource: PlaygroundBluetoothConnectionViewDataSource?

A data source that provides subviews for available peripherals.


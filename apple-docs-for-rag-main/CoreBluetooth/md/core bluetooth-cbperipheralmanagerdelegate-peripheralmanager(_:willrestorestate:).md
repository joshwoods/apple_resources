

- Core Bluetooth
- CBPeripheralManagerDelegate
-  peripheralManager(\_:willRestoreState:) 

Instance Method

# peripheralManager(\_:willRestoreState:)

Tells the delegate the system is about to restore the peripheral manager.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheralManager(
    _ peripheral: CBPeripheralManager,
    willRestoreState dict: [String : Any]
)
```

## Parameters 

`peripheral`  

The peripheral manager undergoing state restoration.

`dict`  

A dictionary that contains information about the peripheral manager, which the system preserved when the app terminated. For the available keys to this dictionary, see Peripheral Manager State Restoration Options.

## Discussion

For apps that opt in to the state preservation and restoration feature, Core Bluetooth invokes this method when relaunching your app into the background to complete some Bluetooth-related task. Use this method to synchronize the state of your app with the state of the Bluetooth system.

## See Also

### Monitoring Changes to the Peripheral Manager’s State

func peripheralManagerDidUpdateState(CBPeripheralManager)

Tells the delegate the peripheral manager’s state updated.

**Required**

Peripheral Manager State Restoration Options

Keys used to specify options when restoring the state of a peripheral manager.


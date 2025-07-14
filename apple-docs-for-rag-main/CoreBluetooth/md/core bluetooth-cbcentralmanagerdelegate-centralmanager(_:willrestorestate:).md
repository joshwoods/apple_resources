

- Core Bluetooth
- CBCentralManagerDelegate
-  centralManager(\_:willRestoreState:) 

Instance Method

# centralManager(\_:willRestoreState:)

Tells the delegate the system is about to restore the central manager, as part of relaunching the app into the background.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func centralManager(
    _ central: CBCentralManager,
    willRestoreState dict: [String : Any]
)
```

## Parameters 

`central`  

The central manager that provides this information.

`dict`  

A dictionary that contains information about the central manager preserved by the system when it terminated the app. For the available keys to this dictionary, see Central Manager State Restoration Options.

## Discussion

This method only applies to apps that opt in to the state preservation and restoration feature of Core Bluetooth. The system invokes this method when relaunching your app into the background to complete some Bluetooth-related task. Use this method to synchronize the state of your app with the state of the Bluetooth system.

## See Also

### Monitoring the Central Manager’s State

func centralManagerDidUpdateState(CBCentralManager)

Tells the delegate the central manager’s state updated.

**Required**


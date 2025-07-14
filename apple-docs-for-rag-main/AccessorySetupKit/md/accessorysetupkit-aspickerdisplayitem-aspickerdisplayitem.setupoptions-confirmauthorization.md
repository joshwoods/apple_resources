

- AccessorySetupKit
- ASPickerDisplayItem
- ASPickerDisplayItem.SetupOptions
-  confirmAuthorization 

Type Property

# confirmAuthorization

An option to require the app to finish accessory authorization before showing the setup view.

iOS 18.0+iPadOS 18.0+

``` source
static var confirmAuthorization: ASPickerDisplayItem.SetupOptions { get }
```

## Discussion

If the accessory supports bluetoothPairingLE, then the app needs to start pairing by accessing a protected GATT characteristic.

## See Also

### Options

static var rename: ASPickerDisplayItem.SetupOptions

An option to ask the person using the app to rename the accessory.

static var finishInApp: ASPickerDisplayItem.SetupOptions

An option to ask the person setting up the accessory to finish additional setup in the app after the accessory is authorized.


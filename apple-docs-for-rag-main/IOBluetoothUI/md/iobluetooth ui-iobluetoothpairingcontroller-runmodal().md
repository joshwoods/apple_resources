

- IOBluetooth UI
- IOBluetoothPairingController
-  runModal() 

Instance Method

# runModal()

Runs the pairing panel in a modal session to allow the user to select a Bluetooth device.

macOS 10.2+

``` source
@MainActor
func runModal() -> Int32
```

## Return Value

Returns kIOBluetoothUISuccess if a successful, validated device selection was made by the user and that device successfully paired. Returns kIOBluetoothUIUserCanceledErr if the user cancelled the panel. These return values are the same as NSRunStoppedResponse and NSRunAbortedResponse respectively. They are the standard values used in a modal session.

## Discussion

The controller will use the panel attributes to filter what devices the user sees. The allowed UUIDs will be used to validate the selection the user makes. Only when a selection has been validated (or the panel cancelled) and the device paired, will this method return.

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

## See Also

### Instance Methods

func addAllowedUUID(IOBluetoothSDPUUID!)

Adds a UUID to the list of UUIDs that are used to validate the user’s selection.

func addAllowedUUIDArray([Any]!)

Adds an array of UUIDs to the list of UUIDs that are used to validate the user’s selection.

func clearAllowedUUIDs()

Resets the controller back to the default state where it will accept any device the user selects.

func getDescriptionText() -> String!

Returns the description text that appears in the device selector panel.

func getOptions() -> IOBluetoothServiceBrowserControllerOptions

Returns the option bits that control the panel’s behavior.

func getPrompt() -> String!

Returns the title of the default/select button in the device selector panel.

func getResults() -> [Any]!

Returns an NSArray of the devices that were paired.

func getSearchAttributes() -> UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!

Returns the search attributes that control the panel’s search/inquiry behavior.

func getTitle() -> String!

Returns the title of the device selector panel.

func setDescriptionText(String!)

Sets the description text that appears in the device selector panel.

func setOptions(IOBluetoothServiceBrowserControllerOptions)

Sets the option bits that control the panel’s behavior.

func setPrompt(String!)

Sets the title of the default/select button in the device selector panel.

func setSearchAttributes(UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!)

Sets the search attributes that control the panel’s search/inquiry behavior.

func setTitle(String!)

Sets the title of the panel when not run as a sheet.


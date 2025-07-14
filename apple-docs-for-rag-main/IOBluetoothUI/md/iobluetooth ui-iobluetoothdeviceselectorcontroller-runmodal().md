

- IOBluetooth UI
- IOBluetoothDeviceSelectorController
-  runModal() 

Instance Method

# runModal()

Runs the device selector panel in a modal session to allow the user to select a Bluetooth device.

macOS 10.2+

``` source
@MainActor
func runModal() -> Int32
```

## Return Value

Returns kIOBluetoothUISuccess if a successful, validated device selection was made by the user. Returns kIOBluetoothUIUserCanceledErr if the user cancelled the panel. These return values are the same as NSRunStoppedResponse and NSRunAbortedResponse respectively. They are the standard values used in a modal session.

## Discussion

The controller will use the panel attributes to filter what devices the user sees. The allowed UUIDs will be used to validate the selection the user makes. Only when a selection has been validated (or the panel cancelled), will this method return.

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

## See Also

### Instance Methods

func addAllowedUUID(IOBluetoothSDPUUID!)

Adds a UUID to the list of UUIDs that are used to validate the user’s selection.

func addAllowedUUIDArray([Any]!)

Adds an array of UUIDs to the list of UUIDs that are used to validate the user’s selection.

func beginSheetModal(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!) -> IOReturn

Runs the device selector panel as a sheet on the target window.

func clearAllowedUUIDs()

Resets the controller back to the default state where it will accept any device the user selects.

func getCancel() -> String!

Returns the title of the default/cancel button in the device selector panel.

func getDescriptionText() -> String!

Returns the description text that appears in the device selector panel.

func getHeader() -> String!

Returns the header text that appears in the device selector panel.

func getOptions() -> IOBluetoothServiceBrowserControllerOptions

Returns the option bits that control the panel’s behavior.

func getPrompt() -> String!

Returns the title of the default/select button in the device selector panel.

func getResults() -> [Any]!

Returns the result of the user’s selection.

func getSearchAttributes() -> UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!

Returns the search attributes that control the panel’s search/inquiry behavior.

func getTitle() -> String!

Returns the title of the device selector panel.

func setCancel(String!)

Sets the title of the default/cancel button in the device selector panel.

func setDescriptionText(String!)

Sets the description text that appears in the device selector panel.

func setHeader(String!)

Sets the header text that appears in the device selector panel.


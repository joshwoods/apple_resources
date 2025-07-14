

- IOBluetooth UI
- IOBluetoothServiceBrowserController
-  getResults() 

Instance Method

# getResults()

Returns the result of the user’s selection.

macOS 10.2+

``` source
@MainActor
func getResults() -> [Any]!
```

## Return Value

Returns an NSArray of IOBluetoothSDPServiceRecord objects corresponding to the user’s selection. If the user cancelled the panel, nil will be returned.

## Discussion

There will only be results if the panel has been run, the user has successfully made a selection and that selection has been validated. If kIOBluetoothUISuccess was returned for the session, there should be valid results. Currently only a single device is allowed to be selected, so the results array will only contain one object. However in the future multiple selection will be supported.

NOTE: This method is only available in macOS 10.2.4 (Bluetooth v1.1) or later.

## See Also

### Instance Methods

func addAllowedUUID(IOBluetoothSDPUUID!)

Adds a UUID to the list of UUIDs that are used to validate the user’s selection.

func addAllowedUUIDArray([Any]!)

Adds an array of UUIDs to the list of UUIDs that are used to validate the user’s selection.

func beginSheetModal(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!) -> IOReturn

Runs the service browser panel as a sheet on the target window.

func clearAllowedUUIDs()

Resets the controller back to the default state where it will accept any device the user selects.

func getDescriptionText() -> String!

Returns the description text that appears in the device selector panel.

func getOptions() -> IOBluetoothServiceBrowserControllerOptions

Returns the option bits that control the panel’s behavior.

func getPrompt() -> String!

Returns the title of the default/select button in the device selector panel.

func getRef() -> Unmanaged&lt;IOBluetoothServiceBrowserControllerRef>!

Returns an IOBluetoothServiceBrowserControllerRef representation of the target IOBluetoothServiceBrowserController object.

func getSearchAttributes() -> UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!

Returns the search attributes that control the panel’s search/inquiry behavior.

func getTitle() -> String!

Returns the title of the device selector panel.

func runModal() -> Int32

Runs the service browser panel in a modal session to allow the user to select a service on a Bluetooth device.

func setDescriptionText(String!)

Sets the description text that appears in the device selector panel.

func setOptions(IOBluetoothServiceBrowserControllerOptions)

Modify the options for the window controller.

func setPrompt(String!)

Sets the title of the default/select button in the device selector panel.

func setSearchAttributes(UnsafePointer&lt;IOBluetoothDeviceSearchAttributes>!)

Sets the search attributes that control the panel’s search/inquiry behavior.


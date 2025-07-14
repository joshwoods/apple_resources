

- IOBluetooth UI
- IOBluetoothDeviceSelectorController
-  setDescriptionText(\_:) 

Instance Method

# setDescriptionText(\_:)

Sets the description text that appears in the device selector panel.

macOS 10.2+

``` source
@MainActor
func setDescriptionText(_ descriptionText: String!)
```

## Parameters 

`descriptionText`  

String that appears in the description section of the device selector panel.

## Discussion

The description text should be localized for best user experience.

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

func runModal() -> Int32

Runs the device selector panel in a modal session to allow the user to select a Bluetooth device.

func setCancel(String!)

Sets the title of the default/cancel button in the device selector panel.

func setHeader(String!)

Sets the header text that appears in the device selector panel.


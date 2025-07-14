

- IOBluetooth UI
- IOBluetoothObjectPushUIController
-  getTitle() 

Instance Method

# getTitle()

Returns the title of the transfer panel.

macOS 10.2+

``` source
@MainActor
func getTitle() -> String!
```

## Return Value

Returns the title of the transfer panel.

## See Also

### Instance Methods

func beginSheetModal(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!) -> IOReturn

Runs the transfer UI as a sheet on the target window.

func getDevice() -> IOBluetoothDevice!

Gets the object representing the remote target device in the transfer.

func isTransferInProgress() -> Bool

Gets state of the transfer

func runModal()

Runs the transfer UI panel in a modal session

func runPanel()

Runs the transfer UI as a panel with no modal session

func setIconImage(NSImage!)

Manually sets the icon used in the panel.

func setTitle(String!)

Sets the title of the panel when not run as a sheet.

func stop()

Stops the transfer UI


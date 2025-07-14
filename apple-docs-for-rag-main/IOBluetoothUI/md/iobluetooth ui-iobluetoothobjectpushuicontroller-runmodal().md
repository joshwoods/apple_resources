

- IOBluetooth UI
- IOBluetoothObjectPushUIController
-  runModal() 

Instance Method

# runModal()

Runs the transfer UI panel in a modal session

macOS 10.2+

``` source
@MainActor
func runModal()
```

## Discussion

Returns when the modal session has ended. This object will call back over the delegate method (above) when the transfer is complete. Users should release the object then. If no delegate is set the object will release itself.

## See Also

### Instance Methods

func beginSheetModal(for: NSWindow!, modalDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!) -> IOReturn

Runs the transfer UI as a sheet on the target window.

func getDevice() -> IOBluetoothDevice!

Gets the object representing the remote target device in the transfer.

func getTitle() -> String!

Returns the title of the transfer panel.

func isTransferInProgress() -> Bool

Gets state of the transfer

func runPanel()

Runs the transfer UI as a panel with no modal session

func setIconImage(NSImage!)

Manually sets the icon used in the panel.

func setTitle(String!)

Sets the title of the panel when not run as a sheet.

func stop()

Stops the transfer UI


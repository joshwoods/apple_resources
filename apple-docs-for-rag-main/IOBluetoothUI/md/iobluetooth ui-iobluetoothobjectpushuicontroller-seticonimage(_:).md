

- IOBluetooth UI
- IOBluetoothObjectPushUIController
-  setIconImage(\_:) 

Instance Method

# setIconImage(\_:)

Manually sets the icon used in the panel.

macOS 10.2+

``` source
@MainActor
func setIconImage(_ image: NSImage!)
```

## Parameters 

`image`  

Image to use as the icon.

## Discussion

The panel icon should be set to the icon of the calling application. If not set, the panel will try to load up the correct icon for the target device, and will default to the icon of the running application on fail.

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

func runModal()

Runs the transfer UI panel in a modal session

func runPanel()

Runs the transfer UI as a panel with no modal session

func setTitle(String!)

Sets the title of the panel when not run as a sheet.

func stop()

Stops the transfer UI


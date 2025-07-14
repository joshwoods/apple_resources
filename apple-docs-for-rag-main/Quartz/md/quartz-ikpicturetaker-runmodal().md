

- Quartz
- IKPictureTaker
-  runModal() 

Instance Method

# runModal()

Opens a modal picture taker dialog.

macOS 10.4+

``` source
@MainActor
func runModal() -> Int
```

## Return Value

Returns `NSOKButton` if the user edits or chooses an image; `NSCancelButton` if the user cancels or does not change the default image.

## See Also

### Creating And Displaying The Picture Taker

class func pictureTaker() -> IKPictureTaker!

Returns a shared `IKPictureTaker` instance, creating it if necessary.

func beginSheet(for: NSWindow!, withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Opens a picture taker as a sheet whose parent is the specified window.

func begin(withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Opens a picture taker pane.

func popUpRecentsMenu(for: NSView!, withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays the Open Recent popup menu associated with the picture taker.




- Quartz
- IKPictureTaker
-  pictureTaker() 

Type Method

# pictureTaker()

Returns a shared `IKPictureTaker` instance, creating it if necessary.

macOS 10.4+

``` source
@MainActor
class func pictureTaker() -> IKPictureTaker!
```

## Return Value

An `IKPictureTaker` object.

## See Also

### Creating And Displaying The Picture Taker

func beginSheet(for: NSWindow!, withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Opens a picture taker as a sheet whose parent is the specified window.

func begin(withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Opens a picture taker pane.

func popUpRecentsMenu(for: NSView!, withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays the Open Recent popup menu associated with the picture taker.

func runModal() -> Int

Opens a modal picture taker dialog.


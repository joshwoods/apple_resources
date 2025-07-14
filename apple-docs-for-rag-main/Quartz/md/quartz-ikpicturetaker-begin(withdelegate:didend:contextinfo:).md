

- Quartz
- IKPictureTaker
-  begin(withDelegate:didEnd:contextInfo:) 

Instance Method

# begin(withDelegate:didEnd:contextInfo:)

Opens a picture taker pane.

macOS 10.4+

``` source
@MainActor
func begin(
    withDelegate delegate: Any!,
    didEnd didEndSelector: Selector!,
    contextInfo: UnsafeMutableRawPointer!
)
```

## Parameters 

`delegate`  

The object that will invoke the selector `didEndSelector` when the picture taker session terminates.

`didEndSelector`  

The selector to invoke when the picture taker session terminates.

`contextInfo`  

Any data that must be passed as an argument to the delegate through `didEndSelector` after the picture taker session terminates.

## Discussion

The `didEndSelector` method should have the following signature:

`- (void)pictureTakerDidEnd:(IKPictureTaker *)sheet returnCode:(NSInteger)returnCode contextInfo:(void *)contextInfo;`

The `returnCode` value is set to `NSOKButton` if the user validates, or to `NSCancelButton` if the user cancels.

## See Also

### Creating And Displaying The Picture Taker

class func pictureTaker() -> IKPictureTaker!

Returns a shared `IKPictureTaker` instance, creating it if necessary.

func beginSheet(for: NSWindow!, withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Opens a picture taker as a sheet whose parent is the specified window.

func popUpRecentsMenu(for: NSView!, withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Displays the Open Recent popup menu associated with the picture taker.

func runModal() -> Int

Opens a modal picture taker dialog.


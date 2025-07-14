

- Quartz
- IKPictureTaker
-  popUpRecentsMenu(for:withDelegate:didEnd:contextInfo:) 

Instance Method

# popUpRecentsMenu(for:withDelegate:didEnd:contextInfo:)

Displays the Open Recent popup menu associated with the picture taker.

macOS 10.4+

``` source
@MainActor
func popUpRecentsMenu(
    for aView: NSView!,
    withDelegate delegate: Any!,
    didEnd didEndSelector: Selector!,
    contextInfo: UnsafeMutableRawPointer!
)
```

## Parameters 

`aView`  

The object that will invoke the selector `didEndSelector` when the picture taker session terminates.

`delegate`  

The selector to invoke when the picture taker session terminates.

`didEndSelector`  

Any data that must be passed as an argument to the delegate through `didEndSelector` after the picture taker session terminates.

`contextInfo`  

An optional context object available to delegates when called.

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

func begin(withDelegate: Any!, didEnd: Selector!, contextInfo: UnsafeMutableRawPointer!)

Opens a picture taker pane.

func runModal() -> Int

Opens a modal picture taker dialog.


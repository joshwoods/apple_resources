

- Screen Saver
- ScreenSaverView
-  configureSheet 

Instance Property

# configureSheet

The window that contains the controls to configure the screen saver.

macOS 10.0+

``` source
@MainActor
var configureSheet: NSWindow? { get }
```

## Discussion

The system runs this window as a sheet, so include buttons that allow the user to end the modal session in which the sheet runs. When the user dismisses the sheet, the controller in charge of the sheet must end the document modal session by calling the NSApplication method endSheet(_:) with the sheet’s window as the argument.

## See Also

### Accessing the configuration sheet

var hasConfigureSheet: Bool

A Boolean value that indicates whether the screen saver has an associated configuration sheet.




- XCUIAutomation
- XCUIRemote
-  press(\_:forDuration:) 

Instance Method

# press(\_:forDuration:)

Sends a press and hold of a button on a physical remote control, holding for the specified duration.

tvOSXcode 16.3+

``` source
@MainActor
func press(
    _ remoteButton: XCUIRemote.Button,
    forDuration duration: TimeInterval
)
```

## Parameters 

`remoteButton`  

The button on the physical remote control that you want to press and hold.

`duration`  

The duration of the button press and hold in seconds.

## See Also

### Pressing remote buttons

func press(XCUIRemote.Button)

Sends a momentary press of a button on a physical remote control.

enum XCUIRemoteButton

A button on a physical remote control.


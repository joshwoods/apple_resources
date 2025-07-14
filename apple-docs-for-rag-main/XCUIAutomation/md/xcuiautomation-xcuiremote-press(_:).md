

- XCUIAutomation
- XCUIRemote
-  press(\_:) 

Instance Method

# press(\_:)

Sends a momentary press of a button on a physical remote control.

tvOSXcode 16.3+

``` source
@MainActor
func press(_ remoteButton: XCUIRemote.Button)
```

## Parameters 

`remoteButton`  

The button on the physical remote control that you want to press.

## See Also

### Pressing remote buttons

func press(XCUIRemote.Button, forDuration: TimeInterval)

Sends a press and hold of a button on a physical remote control, holding for the specified duration.

enum XCUIRemoteButton

A button on a physical remote control.


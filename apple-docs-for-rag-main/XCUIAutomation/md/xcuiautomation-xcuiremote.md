

- XCUIAutomation
-  XCUIRemote 

Class

# XCUIRemote

A class that simulates interaction with a physical remote control.

tvOSXcode 16.3+

``` source
@MainActor
class XCUIRemote
```

## Topics

### Accessing the simulated remote

class var shared: XCUIRemote

The simulated physical remote control.

### Pressing remote buttons

func press(XCUIRemote.Button)

Sends a momentary press of a button on a physical remote control.

func press(XCUIRemote.Button, forDuration: TimeInterval)

Sends a press and hold of a button on a physical remote control, holding for the specified duration.

enum XCUIRemoteButton

A button on a physical remote control.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable


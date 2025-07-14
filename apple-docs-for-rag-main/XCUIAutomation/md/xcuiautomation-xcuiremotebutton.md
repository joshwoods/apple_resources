

- XCUIAutomation
-  XCUIRemoteButton 

Enumeration

# XCUIRemoteButton

A button on a physical remote control.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

**tvOS**

``` source
enum Button
```

**iOS, iPadOS, macOS, visionOS, watchOS**

``` source
enum XCUIRemoteButton
```

## Topics

### Remote buttons

case up

A constant that represents the up button on a remote.

case down

A constant that represents the down button on a remote.

case left

A constant that represents the left button on a remote.

case right

A constant that represents the right button on a remote.

case select

A constant that represents the select button on a remote.

case menu

A constant that represents the menu button on a remote.

case playPause

A constant that represents the play-and-pause button on a remote.

case home

A constant that represents the home button on a remote.

case pageUp

A constant that represents the page up button on a remote.

case pageDown

A constant that represents the page down button on a remote.

case guide

A constant that represents the guide button on a remote.

case fourColors

A constant that represents the color functions button on a remote.

case oneTwoThree

A constant that represents the channel-tuning button on a remote.

case tvProvider

A constant that represents the TV provider button on a remote.

### Initializers

init?(rawValue: UInt)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Pressing remote buttons

func press(XCUIRemote.Button)

Sends a momentary press of a button on a physical remote control.

func press(XCUIRemote.Button, forDuration: TimeInterval)

Sends a press and hold of a button on a physical remote control, holding for the specified duration.


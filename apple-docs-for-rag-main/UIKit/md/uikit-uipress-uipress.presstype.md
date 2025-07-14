

- UIKit
- UIPress
-  UIPress.PressType 

Enumeration

# UIPress.PressType

Constants that represent buttons that a person can press.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
enum PressType
```

## Topics

### Actions

case playPause

A constant that represents the play/pause button.

case select

A constant that represents the select button.

case menu

A constant that represents the menu button.

### Navigation

case upArrow

A constant that represents the up arrow button.

case downArrow

A constant that represents the down arrow button.

case leftArrow

A constant that represents the left arrow button.

case rightArrow

A constant that represents the right arrow button.

case pageDown

A constant that represents the page down button.

case pageUp

A constant that represents the page up button.

### Enumeration Cases

case tvRemoteFourColors

Represents a button on a TV remote labeled with four colors, analogous to the four separate color buttons found on some TV remotes. When this button is pressed, an app should perform the appropriate color action or if there are multiple color actions available provide UI to choose the specific color.

case tvRemoteOneTwoThree

Represents a button on a TV remote labeled with 123. When this button is pressed, an app should provide UI to enter a specific channel number if channel numbers are available. If no channel numbers exist the app should provide UI to toggle channel category filters, search for channels by name or search for currently airing shows.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum Phase

Constants that represent the phases of a button press.


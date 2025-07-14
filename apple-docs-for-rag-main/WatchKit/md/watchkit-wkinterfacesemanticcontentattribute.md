

- WatchKit
-  WKInterfaceSemanticContentAttribute 

Enumeration

# WKInterfaceSemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

watchOS 2.1+

``` source
enum WKInterfaceSemanticContentAttribute
```

## Topics

### Constants

case unspecified

The default value for views. The view is flipped when switching between left-to-right and right-to-left layouts.

case playback

A view representing the playback controls, such as Play, Rewind, or Fast Forward buttons or playhead scrubbers. These views are not flipped when switching between left-to-right and right-to-left layouts.

case spatial

A view representing a directional control, for example a segment control for text alignment, or a D-pad control for a game. These views are not flipped when switching between left-to-right and right-to-left layouts.

case forceLeftToRight

A view that is always displayed using a left-to-right layout.

case forceRightToLeft

A view that is always displayed using a left-to-right layout.

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

### Accessing the Layout Direction

var layoutDirection: WKInterfaceLayoutDirection

The layout direction of the user interface.

class func interfaceLayoutDirection(for: WKInterfaceSemanticContentAttribute) -> WKInterfaceLayoutDirection

Returns the user interface direction for the given semantic content attribute.

enum WKInterfaceLayoutDirection

Specifies the directional flow of the user interface.


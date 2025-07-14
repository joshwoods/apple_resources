

- AppKit
- NSTextInputContext
-  localizedName(forInputSource:) 

Type Method

# localizedName(forInputSource:)

Returns the display name for the given text input source identifier.

macOS 10.6+

``` source
class func localizedName(forInputSource inputSourceIdentifier: NSTextInputSourceIdentifier) -> String?
```

## Parameters 

`inputSourceIdentifier`  

The text input source identifier.

## Return Value

The localized display name for `inputSourceIdentifier`.

## See Also

### Handling Input Sources

func handleEvent(NSEvent) -> Bool

Tells the Cocoa text input system to handle mouse or key events.

func discardMarkedText()

Tells the Cocoa text input system to discard the current conversion session.

func invalidateCharacterCoordinates()

Notifies the Cocoa text input system that the position information previously queried via methods like `firstRectForCharacterRange:actualRange:` needs to be updated.

var keyboardInputSources: [NSTextInputSourceIdentifier]?

The array of keyboard text input source identifier strings available to the receiver. (read-only)

var selectedKeyboardInputSource: NSTextInputSourceIdentifier?

The identifier string for the selected keyboard text input source.

typealias NSTextInputSourceIdentifier


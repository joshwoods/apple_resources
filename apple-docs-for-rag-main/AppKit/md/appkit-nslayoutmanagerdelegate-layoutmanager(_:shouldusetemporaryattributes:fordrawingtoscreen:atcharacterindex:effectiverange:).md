

- AppKit
- NSLayoutManagerDelegate
-  layoutManager(\_:shouldUseTemporaryAttributes:forDrawingToScreen:atCharacterIndex:effectiveRange:) 

Instance Method

# layoutManager(\_:shouldUseTemporaryAttributes:forDrawingToScreen:atCharacterIndex:effectiveRange:)

Asks the delegate whether to use temporary attributes when drawing the text.

macOS 10.5+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    shouldUseTemporaryAttributes attrs: [NSAttributedString.Key : Any] = [:],
    forDrawingToScreen toScreen: Bool,
    atCharacterIndex charIndex: Int,
    effectiveRange effectiveCharRange: NSRangePointer?
) -> [NSAttributedString.Key : Any]?
```

## Parameters 

`layoutManager`  

The layout manager sending the message.

`attrs`  

The temporary attributes currently in effect for the given character range.

`toScreen`  

true if the layout manager is drawing to the screen; otherwise, false.

`charIndex`  

Index of the first character in the range being drawn.

`effectiveCharRange`  

On input and output, the effective range to which the temporary attributes apply.

## Return Value

The temporary attributes for the layout manager to use, or `nil` if no temporary attributes are to be used.

## Discussion

The default behavior, if this method is not implemented, is to use temporary attributes only when drawing to the screen, so an implementation to match that behavior would return `attrs` if `toScreen` is true and `nil` otherwise, without changing `effectiveCharRange`.


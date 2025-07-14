

- AppKit
- NSTextView
-  changeDocumentBackgroundColor(\_:) 

Instance Method

# changeDocumentBackgroundColor(\_:)

An action method used to set the background color.

macOS

``` source
@MainActor
func changeDocumentBackgroundColor(_ sender: Any?)
```

## Parameters 

`sender`  

The control that wants to set the background color.

## Discussion

This method gets the new color by sending a color message to `sender`.

This will only set the background color if allowsDocumentBackgroundColorChangereturns true.

## See Also

### Setting graphics attributes

var backgroundColor: NSColor

The receiver’s background color.

var drawsBackground: Bool

A Boolean value that indicates whether the receiver draws its background.

var allowsDocumentBackgroundColorChange: Bool

A Boolean value that indicates whether the receiver allows its background color to change.


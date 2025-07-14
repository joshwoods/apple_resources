

- AppKit
- NSButtonCell
-  setButtonType(\_:) 

Instance Method

# setButtonType(\_:)

Sets how the button highlights while pressed and how it shows its state.

macOS

``` source
@MainActor
func setButtonType(_ type: NSButton.ButtonType)
```

## Parameters 

`type`  

A constant specifying the type of button. This can be one of the constants defined in NSButton.ButtonType.

## Discussion

The setButtonType(_:) method redisplays the button before returning.

The types available are for the most common button types, which are also accessible in Interface Builder; you can configure different behavior with the highlightsBy and showsStateBy properties.

Note that there is no `-buttonType` method. The set method sets various button properties that together establish the behavior of the type.

## See Also

### Related Documentation

var image: NSImage?

The image displayed by the cell, if any.

var alternateImage: NSImage?

The image the button displays in its alternate state.

### Displaying the Cell

var highlightsBy: NSCell.StyleMask

A set of flags that indicate how the button highlights when it receives a mouse-down event (that is, when the button is pressed).

var showsStateBy: NSCell.StyleMask

The flags that indicate how the button cell shows its alternate state.


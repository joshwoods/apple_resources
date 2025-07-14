

- UIKit
- UITextInput
-  textStyling(at:in:) 

Instance Method

# textStyling(at:in:)

Returns a dictionary with properties that specify how to style the text at a certain location in a document.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func textStyling(
    at position: UITextPosition,
    in direction: UITextStorageDirection
) -> [NSAttributedString.Key : Any]?
```

## Parameters 

`position`  

An object that indicates a location in the text of a document.

`direction`  

The direction of the styling attributes in text storage.

## Return Value

A dictionary whose elements are one or more of the key-value pairs defining text color, font, and background color. See Style dictionary keys for descriptions of these key-value pairs.

## Discussion

Text styling information can affect, for example, the appearance of a correction rectangle.


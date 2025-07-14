

- UIKit
- UITextView
-  init(frame:textContainer:) 

Initializer

# init(frame:textContainer:)

Creates a new text view with the specified text container.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    frame: CGRect,
    textContainer: NSTextContainer?
)
```

## Parameters 

`frame`  

The frame rectangle of the text view.

`textContainer`  

The text container to use for the receiver (can be `nil`).

## Return Value

An initialized text view.

## Discussion

This is the designated initializer for `UITextView` objects.

## See Also

### Initializing the text view

convenience init(usingTextLayoutManager: Bool)

Creates a new text view, with or without a text layout manager depending on the Boolean value you specify.

init?(coder: NSCoder)

Creates a text view from data in an unarchiver.




- UIKit
- UITextView
-  init(usingTextLayoutManager:) 

Initializer

# init(usingTextLayoutManager:)

Creates a new text view, with or without a text layout manager depending on the Boolean value you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
convenience init(usingTextLayoutManager: Bool)
```

## Parameters 

`usingTextLayoutManager`  

A Boolean value that indicates whether the framework should create the text view with an NSTextLayoutManager.

## See Also

### Initializing the text view

init(frame: CGRect, textContainer: NSTextContainer?)

Creates a new text view with the specified text container.

init?(coder: NSCoder)

Creates a text view from data in an unarchiver.




- UIKit
- UITextView
-  init(coder:) 

Initializer

# init(coder:)

Creates a text view from data in an unarchiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Initializing the text view

init(frame: CGRect, textContainer: NSTextContainer?)

Creates a new text view with the specified text container.

convenience init(usingTextLayoutManager: Bool)

Creates a new text view, with or without a text layout manager depending on the Boolean value you specify.


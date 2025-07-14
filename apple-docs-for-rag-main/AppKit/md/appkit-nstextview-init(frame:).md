

- AppKit
- NSTextView
-  init(frame:) 

Initializer

# init(frame:)

Initializes a text view.

macOS

``` source
@MainActor
init(frame frameRect: NSRect)
```

## Parameters 

`frameRect`  

The frame rectangle of the text view.

## Return Value

An initialized text view.

## Discussion

This method creates the entire collection of objects associated with a text view—its text container, layout manager, and text storage—and invokes init(frame:textContainer:).

This method creates the text web in such a manner that the text view is the principal owner of the objects in the web.

## See Also

### Creating a text view

init(frame: NSRect, textContainer: NSTextContainer?)

Initializes a text view.

convenience init(usingTextLayoutManager: Bool)

init?(coder: NSCoder)

Initializes a text view with data in an unarchiver.


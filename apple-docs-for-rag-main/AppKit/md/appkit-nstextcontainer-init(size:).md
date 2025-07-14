

- AppKit
- NSTextContainer
-  init(size:) 

Initializer

# init(size:)

Initializes a text container with a specified bounding rectangle.

macOS 10.11+

``` source
init(size: CGSize)
```

## Parameters 

`size`  

The size of the text container’s bounding rectangle.

## Discussion

The new text container must be added to an NSLayoutManager object before it can be used. The text container must also have an associated NSTextView object for text to be displayed. This method is the designated initializer for the `NSTextContainer` class.

## See Also

### Creating a text container

init(coder: NSCoder)

Creates a text container from data in an unarchiver.


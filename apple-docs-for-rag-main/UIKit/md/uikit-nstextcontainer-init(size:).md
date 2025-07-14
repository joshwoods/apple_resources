

- UIKit
- NSTextContainer
-  init(size:) 

Initializer

# init(size:)

Initializes a text container with a specified bounding rectangle.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
init(size: CGSize)
```

## Parameters 

`size`  

The size of the text container’s bounding rectangle.

## Return Value

The size of the text container’s bounding rectangle.

## Discussion

The new text container must be added to an NSLayoutManager object before it can be used. The text container must also have an associated NSTextView object for text to be displayed. This method is the designated initializer for the `NSTextContainer` class.

## See Also

### Related Documentation

Text Layout Programming Guide

Cocoa Text Architecture Guide

func addTextContainer(NSTextContainer)

Appends the specified text container to the series of text containers where the layout manager arranges text.

Text System Storage Layer Overview

### Creating a text container

init(coder: NSCoder)

Creates a text container from data in an unarchiver.




- UIKit
- NSTextListElement
-  init(parent:textList:contents:markerAttributes:children:) 

Initializer

# init(parent:textList:contents:markerAttributes:children:)

Creates a text list element with the parent, list elements, nesting level, and marker attributes you provide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    parent: NSTextListElement?,
    textList: NSTextList,
    contents: NSAttributedString?,
    markerAttributes: [NSAttributedString.Key : Any]? = nil,
    children: [NSTextListElement]?
)
```

## Parameters 

`parent`  

The parent `NSTextListElement` of this element, if any.

`textList`  

The NSTextList to add elements to.

`contents`  

An NSAttributedString that contains the contents of the text list element.

`markerAttributes`  

A dictionary of NSAttributedString.Key keys and IDs that describe the marker attributes.

`children`  

An array of NSTextListElement elements.

## See Also

### Create a text list element

convenience init?(children: [NSTextListElement], textList: NSTextList, nestingLevel: Int)

Creates a text list element with the list elements and nesting level you provide.

convenience init(contents: NSAttributedString, markerAttributes: [NSAttributedString.Key : Any]?, textList: NSTextList, children: [NSTextListElement]?)

Creates a text list element with the list elements, nesting level, and marker attributes you provide.


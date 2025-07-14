

- UIKit
- NSTextListElement
-  init(children:textList:nestingLevel:) 

Initializer

# init(children:textList:nestingLevel:)

Creates a text list element with the list elements and nesting level you provide.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
convenience init?(
    children: [NSTextListElement],
    textList: NSTextList,
    nestingLevel: Int
)
```

## Parameters 

`children`  

An array of NSTextListElement elements.

`textList`  

The NSTextList to add elements to.

`nestingLevel`  

An integer value that describes the level of nesting of these elements.

## See Also

### Create a text list element

convenience init(contents: NSAttributedString, markerAttributes: [NSAttributedString.Key : Any]?, textList: NSTextList, children: [NSTextListElement]?)

Creates a text list element with the list elements, nesting level, and marker attributes you provide.

init(parent: NSTextListElement?, textList: NSTextList, contents: NSAttributedString?, markerAttributes: [NSAttributedString.Key : Any]?, children: [NSTextListElement]?)

Creates a text list element with the parent, list elements, nesting level, and marker attributes you provide.


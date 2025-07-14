

- AppKit
- NSTextListElement
-  init(contents:markerAttributes:textList:children:) 

Initializer

# init(contents:markerAttributes:textList:children:)

Creates a text list element with the list elements, nesting level, and marker attributes you provide.

macOS 13.0+

``` source
convenience init(
    contents: NSAttributedString,
    markerAttributes: [NSAttributedString.Key : Any]? = nil,
    textList: NSTextList,
    children: [NSTextListElement]?
)
```

## Parameters 

`contents`  

An NSAttributedString that contains the contents of the text list element.

`markerAttributes`  

A dictionary of NSAttributedString.Key keys and IDs that describe the marker attributes.

`textList`  

The NSTextList to add elements to.

`children`  

An array of NSTextListElement elements.

## See Also

### Create a text list element

convenience init?(children: [NSTextListElement], textList: NSTextList, nestingLevel: Int)

Creates a text list element with the list elements and nesting level you provide.

init(parent: NSTextListElement?, textList: NSTextList, contents: NSAttributedString?, markerAttributes: [NSAttributedString.Key : Any]?, children: [NSTextListElement]?)

Creates a text list element with the parent, list elements, nesting level, and marker attributes you provide.


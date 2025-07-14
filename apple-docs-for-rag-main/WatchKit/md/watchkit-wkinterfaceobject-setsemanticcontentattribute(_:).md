

- WatchKit
- WKInterfaceObject
-  setSemanticContentAttribute(\_:) 

Instance Method

# setSemanticContentAttribute(\_:)

Sets the semantic description of the object’s contents, used to determine whether its content should be flipped when switching between left-to-right and right-to-left layouts.

watchOS 2.1+

``` source
func setSemanticContentAttribute(_ semanticContentAttribute: WKInterfaceSemanticContentAttribute)
```

## Parameters 

`semanticContentAttribute`  

The object’s semantic content attribute. For a list of possible values, see WKInterfaceSemanticContentAttribute.

## Discussion

Some objects should not flip when switching between left-to-right and right-to-left layouts. Typically, this occurs because the object is part of the playback controls or represents physical directions (up, down, left, right) that don’t change. Instead of thinking about whether or not an object should change its orientation, select the semantic content attribute that best describes the object.

For example, set the semantic content attribute on a WKInterfaceGroup object to control whether the group should flip the horizontal ordering of its contents when moving between left-to-right and right-to-left languages.


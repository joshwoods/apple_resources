

- Foundation
- ListFormatter
-  string(for:) 

Instance Method

# string(for:)

Creates a formatted string for an array of items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func string(for obj: Any?) -> String?
```

## Parameters 

`obj`  

An array of objects to format as a list.

## Return Value

A formatted string representing the list of objects in an array. Returns `nil` if the formatter can’t generate a description for all objects in the array, or if `obj` is `nil`.

## Discussion

The list formatter uses itemFormatter to format each item in the array. If itemFormatter doesn’t apply to a particular item, the list formatter falls back to the item’s description(withLocale:) or localizedDescription if implemented. If those methods aren’t implemented, the formatter uses description instead.

## See Also

### Converting Arrays to Formatted Lists

func string(from: [Any]) -> String?

Creates a formatted string for an array of items.

class func localizedString(byJoining: [String]) -> String

Constructs a formatted string from an array of strings that uses the list format specific to the current locale.




- UIKit
- UITextInputTokenizer
-  position(from:toBoundary:inDirection:) 

Instance Method

# position(from:toBoundary:inDirection:)

Return the next text position at a boundary of a text unit of the given granularity in a given direction.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func position(
    from position: UITextPosition,
    toBoundary granularity: UITextGranularity,
    inDirection direction: UITextDirection
) -> UITextPosition?
```

**Required**

## Parameters 

`position`  

A text-position object that represents a location in a document.

`granularity`  

A constant that indicates a certain granularity of text unit.

`direction`  

A constant that indicates a direction relative to `position`. The constant can be of type UITextStorageDirection or UITextLayoutDirection.

## Return Value

The next boundary position of a text unit of the given granularity in the given direction, or `nil` if there is no such position.


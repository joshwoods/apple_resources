

- UIKit
- UITextInputTokenizer
-  isPosition(\_:withinTextUnit:inDirection:) 

Instance Method

# isPosition(\_:withinTextUnit:inDirection:)

Return whether a text position is within a text unit of a specified granularity in a specified direction.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func isPosition(
    _ position: UITextPosition,
    withinTextUnit granularity: UITextGranularity,
    inDirection direction: UITextDirection
) -> Bool
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

true if the text position is within a text unit of the specified granularity in the specified direction; otherwise, return false. If the text position is *at* a boundary, return true only if the boundary is part of the text unit in the given direction.

## See Also

### Determining text positions relative to unit boundaries

func isPosition(UITextPosition, atBoundary: UITextGranularity, inDirection: UITextDirection) -> Bool

Return whether a text position is at a boundary of a text unit of a specified granularity in a specified direction.

**Required**


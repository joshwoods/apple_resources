

- UIKit
- UITextInputTokenizer
-  isPosition(\_:atBoundary:inDirection:) 

Instance Method

# isPosition(\_:atBoundary:inDirection:)

Return whether a text position is at a boundary of a text unit of a specified granularity in a specified direction.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func isPosition(
    _ position: UITextPosition,
    atBoundary granularity: UITextGranularity,
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

true if the text position is at the given text-unit boundary in the given direction; false if it is not at the boundary.

## See Also

### Determining text positions relative to unit boundaries

func isPosition(UITextPosition, withinTextUnit: UITextGranularity, inDirection: UITextDirection) -> Bool

Return whether a text position is within a text unit of a specified granularity in a specified direction.

**Required**


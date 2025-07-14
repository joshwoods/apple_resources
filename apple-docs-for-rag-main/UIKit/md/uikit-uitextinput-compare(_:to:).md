

- UIKit
- UITextInput
-  compare(\_:to:) 

Instance Method

# compare(\_:to:)

Returns how one text position compares to another text position.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func compare(
    _ position: UITextPosition,
    to other: UITextPosition
) -> ComparisonResult
```

**Required**

## Parameters 

`position`  

A custom object that represents a location within a document.

`other`  

A custom object that represents another location within a document.

## Return Value

A value that indicates whether the two text positions are identical or whether one is before the other.

## See Also

### Evaluating text positions

func offset(from: UITextPosition, to: UITextPosition) -> Int

Returns the number of UTF-16 characters between one text position and another text position.

**Required**


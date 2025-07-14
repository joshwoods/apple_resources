

- UIKit
- UITextInput
-  offset(from:to:) 

Instance Method

# offset(from:to:)

Returns the number of UTF-16 characters between one text position and another text position.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func offset(
    from: UITextPosition,
    to toPosition: UITextPosition
) -> Int
```

**Required**

## Parameters 

`from`  

A custom object that represents a location within a document.

`toPosition`  

A custom object that represents another location within document.

## Return Value

The number of UTF-16 characters between `fromPosition` and `toPosition`.

## See Also

### Evaluating text positions

func compare(UITextPosition, to: UITextPosition) -> ComparisonResult

Returns how one text position compares to another text position.

**Required**


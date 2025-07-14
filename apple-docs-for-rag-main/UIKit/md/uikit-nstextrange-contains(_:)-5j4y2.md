

- UIKit
- NSTextRange
-  contains(\_:) 

Instance Method

# contains(\_:)

Determines if the text range you specify is in the current text range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func contains(_ textRange: NSTextRange) -> Bool
```

## Parameters 

`textRange`  

An NSTextRange.

## Return Value

Returns `true` if the range you provide is in the current range; otherwise `false`.

## See Also

### Finding text within the text range

func contains(any NSTextLocation) -> Bool

Determines if the text location you specify is in the current text range.


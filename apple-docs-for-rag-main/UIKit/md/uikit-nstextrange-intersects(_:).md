

- UIKit
- NSTextRange
-  intersects(\_:) 

Instance Method

# intersects(\_:)

Determines if two ranges intersect.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func intersects(_ textRange: NSTextRange) -> Bool
```

## Parameters 

`textRange`  

The range used to compare against the current range to evaluate for differences.

## Return Value

Returns `true` if the ranges intersect.

## See Also

### Comparing text ranges

func intersection(NSTextRange) -> Self?

Returns the range, if any, where two text ranges intersect.

func isEqual(to: NSTextRange) -> Bool

Compares two text ranges.

func union(NSTextRange) -> Self

Returns a new text range by forming the union with the text range you provide.


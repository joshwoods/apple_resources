

- AppKit
- NSTextRange
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Compares two text ranges.

macOS 12.0+

``` source
func isEqual(to textRange: NSTextRange) -> Bool
```

## Parameters 

`textRange`  

The range used to compare against the current range to evaluate for differences.

## Return Value

Returns `true` if the ranges are equal.

## See Also

### Comparing text ranges

func intersection(NSTextRange) -> Self?

Returns the range, if any, where two text ranges intersect.

func intersects(NSTextRange) -> Bool

Determines if two ranges intersect.

func union(NSTextRange) -> Self

Returns a new text range by forming the union with the text range you provide.


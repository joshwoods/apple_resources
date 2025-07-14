

- UIKit
- NSTextRange
-  union(\_:) 

Instance Method

# union(\_:)

Returns a new text range by forming the union with the text range you provide.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func union(_ textRange: NSTextRange) -> Self
```

## Parameters 

`textRange`  

The range to use to create the union.

## Return Value

An NSTextRange that represent the union of the two ranges.

## See Also

### Comparing text ranges

func intersection(NSTextRange) -> Self?

Returns the range, if any, where two text ranges intersect.

func intersects(NSTextRange) -> Bool

Determines if two ranges intersect.

func isEqual(to: NSTextRange) -> Bool

Compares two text ranges.


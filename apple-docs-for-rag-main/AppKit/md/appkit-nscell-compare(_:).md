

- AppKit
- NSCell
-  compare(\_:) 

Instance Method

# compare(\_:)

Compares the string values of the receiver another cell, disregarding case.

macOS

``` source
@MainActor
func compare(_ otherCell: Any) -> ComparisonResult
```

## Parameters 

`otherCell`  

The cell to compare against the receiver. This parameter must be of type `NSCell`; if it is not, this method raises `NSBadComparisonException`.

This value must not be `nil`. If the value is `nil`, the behavior is undefined and may change in future versions of macOS.

## Return Value

`NSOrderedAscending` if the string value of the receiver precedes the string value of `otherCell` in lexical ordering, `NSOrderedSame` if the string values are equivalent in lexical value, and `NSOrderedDescending` string value of the receiver follows the string value of `otherCell` in lexical ordering.


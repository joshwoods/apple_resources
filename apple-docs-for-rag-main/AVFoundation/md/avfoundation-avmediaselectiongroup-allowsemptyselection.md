

- AVFoundation
- AVMediaSelectionGroup
-  allowsEmptySelection 

Instance Property

# allowsEmptySelection

A Boolean value that indicates whether it’s possible to present none of the options in the group when an associated player item is played.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var allowsEmptySelection: Bool { get }
```

## Discussion

If the value of this property is true, you can deselect all of the available media options in the group by passing `nil` as the specified AVMediaSelectionOption object to select(_:in:).


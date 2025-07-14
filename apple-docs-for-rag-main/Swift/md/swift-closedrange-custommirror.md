

- Swift
- ClosedRange
-  customMirror 

Instance Property

# customMirror

The custom mirror for this instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var customMirror: Mirror { get }
```

Available when `Bound` conforms to `Comparable`.

## Discussion

If this type has value semantics, the mirror should be unaffected by subsequent mutations of the instance.

## See Also

### Describing a Range

var description: String

A textual representation of the range.

var debugDescription: String

A textual representation of the range, suitable for debugging.


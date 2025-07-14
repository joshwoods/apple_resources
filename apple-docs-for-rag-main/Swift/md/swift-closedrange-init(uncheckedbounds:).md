

- Swift
- ClosedRange
-  init(uncheckedBounds:) 

Initializer

# init(uncheckedBounds:)

Creates an instance with the given bounds.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(uncheckedBounds bounds: (lower: Bound, upper: Bound))
```

## Parameters 

`bounds`  

A tuple of the lower and upper bounds of the range.

## Discussion

Because this initializer does not perform any checks, it should be used as an optimization only when you are absolutely certain that `lower` is less than or equal to `upper`. Using the closed range operator (`...`) to form `ClosedRange` instances is preferred.

## See Also

### Infrequently Used Functionality

var hashValue: Int

The hash value.


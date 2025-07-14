

- Core Image
- CIFilterShape
-  init(rect:) 

Initializer

# init(rect:)

Initializes a filter shape object with a rectangle.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init(rect r: CGRect)
```

## Parameters 

`r`  

A rectangle. Core Image uses the rectangle specified by integer parts of the values in the `CGRect` data structure.

## Return Value

An initialized CIFilterShape object, or `nil` if the method fails.

## See Also

### Related Documentation

+ shapeWithRect:

Creates a filter shape object and initializes it with a rectangle.


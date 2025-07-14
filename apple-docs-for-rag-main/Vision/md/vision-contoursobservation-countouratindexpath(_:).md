

- Vision
- ContoursObservation
-  countourAtIndexPath(\_:) 

Instance Method

# countourAtIndexPath(\_:)

Retrieves the contour object at the specified index, irrespective of hierarchy.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
func countourAtIndexPath(_ indexPath: IndexPath) -> ContoursObservation.Contour?
```

## Parameters 

`indexPath`  

The index of the contour to retrieve. Valid values are in the range of `0` to `contourCount - 1`.

## Return Value

The contour object at the specified index path, or \`nil\` if the index path is invalid.

## See Also

### Getting the contours

struct Contour

An object that represents a detected contour in an image.

func contourAtIndex(Int) -> ContoursObservation.Contour?

Retrieves the contour object at the specified index, irrespective of hierarchy.


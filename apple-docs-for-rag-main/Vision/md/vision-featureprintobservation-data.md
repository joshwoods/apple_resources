

- Vision
- FeaturePrintObservation
-  data 

Instance Property

# data

The feature print data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
let data: Data
```

## Discussion

Vision divides the data into separate elements. Determine the type of element using `elementType`, and the number of elements using `elementCount`.

## See Also

### Inspecting an observation

let elementCount: Int

The total number of elements in the data.

let elementType: ElementType

The type of each element in the data.

enum ElementType

The type of element in feature print data.


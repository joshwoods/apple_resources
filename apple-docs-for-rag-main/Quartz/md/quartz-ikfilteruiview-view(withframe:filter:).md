

- Quartz
- IKFilterUIView
-  view(withFrame:filter:) 

Type Method

# view(withFrame:filter:)

Creates a view that contains controls for the input parameters of a filter.

macOS 10.4+

``` source
@MainActor
class func view(
    withFrame frameRect: NSRect,
    filter inFilter: CIFilter!
) -> Any!
```

## Parameters 

`frameRect`  

The rectangle that defines the area of the view.

`inFilter`  

A Core Image filter. The view retains the filter.

## Return Value

An `IKFilterUIView` object that contains controls for the input parameters of the provided filter.

## See Also

### Creating and Initializing a Filter UI View

init!(frame: NSRect, filter: CIFilter!)

Initializes a view that contains controls for the input parameters of a filter.


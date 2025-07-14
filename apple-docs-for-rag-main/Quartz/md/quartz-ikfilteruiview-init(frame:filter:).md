

- Quartz
- IKFilterUIView
-  init(frame:filter:) 

Initializer

# init(frame:filter:)

Initializes a view that contains controls for the input parameters of a filter.

macOS 10.4+

``` source
@MainActor
init!(
    frame frameRect: NSRect,
    filter inFilter: CIFilter!
)
```

## Parameters 

`frameRect`  

The rectangle that defines the area of the view.

`inFilter`  

A Core Image filter. The view retains the filter.

## Return Value

The `IKFilterUIView` object initialized with controls for the input parameters of the provided filter.

## See Also

### Creating and Initializing a Filter UI View

class func view(withFrame: NSRect, filter: CIFilter!) -> Any!

Creates a view that contains controls for the input parameters of a filter.


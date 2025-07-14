

- Quartz
- IKImageView
-  setOverlay(\_:forType:) 

Instance Method

# setOverlay(\_:forType:)

Sets an overlay type for a Core Animation layer.

macOS 10.5+

``` source
@MainActor
func setOverlay(
    _ layer: CALayer!,
    forType layerType: String!
)
```

## Parameters 

`layer`  

A Core Animation layer object.

`layerType`  

A layer type. See Overlay Types.

## See Also

### Working With Core Animation

func overlay(forType: String!) -> CALayer!

Returns the Core Animation layer associated with a layer type.


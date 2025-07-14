

- Quartz
- IKImageView
-  overlay(forType:) 

Instance Method

# overlay(forType:)

Returns the Core Animation layer associated with a layer type.

macOS 10.5+

``` source
@MainActor
func overlay(forType layerType: String!) -> CALayer!
```

## Parameters 

`layerType`  

A layer type. See Overlay Types.

## Return Value

The Core Animation layer.

## See Also

### Working With Core Animation

func setOverlay(CALayer!, forType: String!)

Sets an overlay type for a Core Animation layer.


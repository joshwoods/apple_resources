

- Compositor Services
- LayerRenderer
-  device 

Instance Property

# device

The GPU device that the layer renderer uses for drawing operations

visionOS 1.0+

``` source
var device: any MTLDevice { get }
```

## Discussion

You can inspect the device for any information you might need. The system uses it to create the textures for drawing, and also to create synchronization events for the layer.


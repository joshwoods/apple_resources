

- Core Animation
- CALayerContentsFilter
-  trilinear 

Type Property

# trilinear

Trilinear minification filter. Enables mipmap generation. Some renderers may ignore this, or impose additional restrictions, such as source images requiring power-of-two dimensions.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
static let trilinear: CALayerContentsFilter
```

## See Also

### Constants

static let linear: CALayerContentsFilter

Linear interpolation filter.

static let nearest: CALayerContentsFilter

Nearest neighbor interpolation filter.




- AVFoundation
- AVCaptionRenderer
-  bounds 

Instance Property

# bounds

The drawing bounds of caption scenes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var bounds: CGRect { get set }
```

## Discussion

Set this property value before drawing. The renderer uses the value in each call to render(in:for:), until you change it to a new value.

## See Also

### Configuring the Renderer

var captions: [AVCaption]

The captions to render.


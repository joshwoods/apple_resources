

- AppKit
- NSVisualEffectView
-  material 

Instance Property

# material

The material shown by the visual effect view.

macOS 10.10+

``` source
@MainActor
var material: NSVisualEffectView.Material { get set }
```

## Discussion

The default value is NSVisualEffectView.Material.appearanceBased; the material updates to the correct material based on the appearance set on this view.

## See Also

### Specifying the Background Material

enum Material

Constants to specify the material shown by the visual effect view.


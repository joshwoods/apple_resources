

- AppKit
- NSColorPicker
-  init(pickerMask:colorPanel:) 

Initializer

# init(pickerMask:colorPanel:)

Initializes the color picker with the specified color panel and color picker mode mask.

macOS

``` source
@MainActor
init?(
    pickerMask mask: Int,
    colorPanel owningColorPanel: NSColorPanel
)
```

## Parameters 

`mask`  

The color picker mask.

`owningColorPanel`  

The `NSColorPanel` that owns the color picker. This value is cached so it can be accessed using the colorPanel property.

## Return Value

An initialized color picker object.

## Discussion

Override this method to respond to the values in `mask` or do other custom initialization. If you override this method in a subclass, you should forward the message to `super` as part of the implementation.

## See Also

### Related Documentation

var colorPanel: NSColorPanel

The color panel instance that owns the color picker.

Color Programming Topics




- AVFoundation
- AVCapturePhotoSettings
-  embedsPortraitEffectsMatteInPhoto 

Instance Property

# embedsPortraitEffectsMatteInPhoto

Specifies whether the portrait effects matte captured with ths photo should be written to the photo’s file structure.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var embedsPortraitEffectsMatteInPhoto: Bool { get set }
```

## Discussion

The default is true, which tells AV Foundation to embed the portrait effects matte images as HEIF and JPEG in the photo.

This property is ignored if isPortraitEffectsMatteDeliveryEnabled is set to false. AV Foundation includes the portrait effects matte only if both this property and isPortraitEffectsMatteDeliveryEnabled are set to true.

## See Also

### Capturing Portrait Effects Matte

var isPortraitEffectsMatteDeliveryEnabled: Bool

Specifies whether a portrait effects matte should be captured along with the photo.


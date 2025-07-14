

- AVFoundation
- AVCapturePhotoSettings
-  isPortraitEffectsMatteDeliveryEnabled 

Instance Property

# isPortraitEffectsMatteDeliveryEnabled

Specifies whether a portrait effects matte should be captured along with the photo.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isPortraitEffectsMatteDeliveryEnabled: Bool { get set }
```

## Discussion

The default is `NO`. Set to `YES` if you wish to receive a portrait effects matte with your photo. AVFoundation throws an exception if isPortraitEffectsMatteDeliveryEnabled is not set to `YES`, or if your delegate doesn’t respond to the photoOutput(_:didFinishProcessingPhoto:error:) selector.

Important

Portrait effects matte generation requires depth data to be present, so you must also set isDepthDataDeliveryEnabled to `YES`.

Setting this property to `YES` doen’t guarantee that a portrait effects matte will be present in the resulting AVCapturePhoto. The matte is primarily used to improve the rendering quality of portrait effects on the image. If the photo’s content lacks a clear foreground subject, no portrait effects matte is generated, and the property returns `nil`. Setting this property to `YES` may add significant processing time to the delivery of your photoOutput(_:didFinishProcessingPhoto:error:) callback.

## See Also

### Capturing Portrait Effects Matte

var embedsPortraitEffectsMatteInPhoto: Bool

Specifies whether the portrait effects matte captured with ths photo should be written to the photo’s file structure.


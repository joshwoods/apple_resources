

- AVFoundation
- AVCapturePhotoOutput
-  capturePhoto(with:delegate:) 

Instance Method

# capturePhoto(with:delegate:)

Initiates a photo capture using the specified settings.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func capturePhoto(
    with settings: AVCapturePhotoSettings,
    delegate: any AVCapturePhotoCaptureDelegate
)
```

## Parameters 

`settings`  

The settings for the photo capture, such as the output pixel format and flash mode. This method copies the provided AVCapturePhotoSettings object, so future changes to that object do not affect the capture in progress.

Important

It is illegal to reuse a AVCapturePhotoSettings instance for multiple captures. Calling this method throws an exception (invalidArgumentException) if the `settings` object’s uniqueID value matches that of any previously used settings object.

`delegate`  

A delegate object to receive messages about capture progress and results. The photo output calls your delegate methods as the photo advances from capture to processing to delivery of finished images.

## Mentioned in 

Capturing Photos in RAW and Apple ProRAW Formats

Tracking Photo Capture Progress

Capturing Photos with Depth

Capturing and Saving Live Photos

Setting Up a Capture Session

## Discussion

Use this method for all variations of still photography, including single photo capture, RAW format capture (with or without a secondary format such as JPEG), bracketed capture of multiple images, and Live Photo capture.

When you call this method, the photo output validates the properties of your `settings` object to ensure deterministic behavior. For example, the flashMode setting must specify a value that is present in the photo output’s supportedFlashModes array. See each property’s description in the AVCapturePhotoSettings class reference for detailed validation rules.


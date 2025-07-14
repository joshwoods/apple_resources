

- AVFoundation
- AVCaptureInput
- AVCaptureInput.Port
-  formatDescriptionDidChangeNotification 

Type Property

# formatDescriptionDidChangeNotification

A notification the system posts when the capture input port’s format description changes.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
class let formatDescriptionDidChangeNotification: NSNotification.Name
```

## Discussion

The notification’s object property contains the AVCaptureInput.Port object whose format changed.


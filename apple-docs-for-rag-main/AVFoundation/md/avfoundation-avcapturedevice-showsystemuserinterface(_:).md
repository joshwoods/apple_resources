

- AVFoundation
- AVCaptureDevice
-  showSystemUserInterface(\_:) 

Type Method

# showSystemUserInterface(\_:)

Displays the system’s user interface to configure video effects or microphone modes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+

``` source
class func showSystemUserInterface(_ systemUserInterface: AVCaptureDevice.SystemUserInterface)
```

## Parameters 

`systemUserInterface`  

The system user interface to present.

## Discussion

Use this method to prompt the user to make changes to Video Effects (such as Center Stage or Portrait Effect) or Microphone Modes. It presents the system user interface and deep links to the appropriate module.

Calling this method isn’t a blocking operation. After the system presents the indicated user interface, control returns immediately to the app.

## See Also

### Presenting the Configuration User Interface

enum SystemUserInterface

Constants that describe the capture device configuration user interfaces.


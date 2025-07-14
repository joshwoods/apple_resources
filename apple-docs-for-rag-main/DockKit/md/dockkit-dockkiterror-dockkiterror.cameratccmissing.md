

- DockKit
- DockKitError
-  DockKitError.cameraTCCMissing 

Case

# DockKitError.cameraTCCMissing

The camera terms and conditions are missing.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
case cameraTCCMissing
```

## Discussion

In order for DockKit to access the camera, a person must accept the terms and conditions. If you receive this error, show an alert indicating that terms and conditions are necessary.


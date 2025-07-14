

- ScreenCaptureKit
- SCContentSharingPicker
-  shared 

Type Property

# shared

The system-provided picker UI instance for capturing display and audio content from someone’s Mac.

Mac Catalyst 18.2+macOS 14.0+

``` source
class var shared: SCContentSharingPicker { get }
```

## Discussion

Important

Use this shared instance of the system picker rather than creating your own.

The picker gives a person control over what information on their Mac they wish to let your app view or record such as specific applications, displays, and windows.


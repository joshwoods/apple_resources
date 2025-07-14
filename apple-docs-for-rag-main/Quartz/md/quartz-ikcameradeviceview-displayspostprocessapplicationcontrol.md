

- Quartz
- IKCameraDeviceView
-  displaysPostProcessApplicationControl 

Instance Property

# displaysPostProcessApplicationControl

Displays whether the post process application control should be displayed.

macOS 10.6+

``` source
@MainActor
var displaysPostProcessApplicationControl: Bool { get set }
```

## Discussion

The post process application is only relevant when the transferMode is set to IKCameraDeviceViewTransferMode.fileBased.

## See Also

### Getting and Setting the Post Processing Application

var postProcessApplication: URL!

The URL of the application used to post process the image.


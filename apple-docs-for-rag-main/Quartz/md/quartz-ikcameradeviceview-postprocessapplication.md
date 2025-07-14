

- Quartz
- IKCameraDeviceView
-  postProcessApplication 

Instance Property

# postProcessApplication

The URL of the application used to post process the image.

macOS 10.6+

``` source
@MainActor
var postProcessApplication: URL! { get set }
```

## Discussion

The post process application is only relevant when the transferMode is set to IKCameraDeviceViewTransferMode.fileBased.

## See Also

### Getting and Setting the Post Processing Application

var displaysPostProcessApplicationControl: Bool

Displays whether the post process application control should be displayed.


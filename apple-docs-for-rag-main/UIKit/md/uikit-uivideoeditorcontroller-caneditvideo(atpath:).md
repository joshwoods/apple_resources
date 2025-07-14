

- UIKit
- UIVideoEditorController
-  canEditVideo(atPath:) 

Type Method

# canEditVideo(atPath:)

Returns a Boolean value indicating whether a video file can be edited.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func canEditVideo(atPath videoPath: String) -> Bool
```

## Parameters 

`videoPath`  

The filesystem path to the video file you want to edit.

## Return Value

true if the specified video file can be edited on the current device or false if it cannot.

## Discussion

Video editing requires the presence of specific hardware and is available only for specific file formats. Use this method to check whether video editing is available for a given video file, before you create a video editor.


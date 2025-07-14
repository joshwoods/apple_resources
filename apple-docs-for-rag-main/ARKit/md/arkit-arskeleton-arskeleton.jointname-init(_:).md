

- ARKit
- ARSkeleton
- ARSkeleton.JointName
-  init(\_:) 

Initializer

# init(\_:)

Returns a joint name that corresponds to a key point defined in a human body pose.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
init?(_ recognizedPointKey: VNRecognizedPointKey)
```

## Parameters 

`recognizedPointKey`  

The argument key point.

## Discussion

This function matches human body key points defined by the Vision framework with joint names defined by ARKit. This function may return `nil` if the key point doesn’t map to a joint name. For more information about key points, see Detecting Human Body Poses in Images.

## See Also

### Creating a Joint Name

init(rawValue: String)

Creates a new joint name.

struct VNRecognizedPointKey

The data type for all recognized point keys.




- ImageCaptureCore
- ICCameraItem
-  userData 

Instance Property

# userData

A mutable dictionary to store arbitrary key-value pairs associated with a camera item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
var userData: NSMutableDictionary? { get }
```

## Discussion

View objects can bind to this object to store “house-keeping” information.




- AVFoundation
- AVPlayerLooper
-  error 

Instance Property

# error

An error that describes the reason looping failed.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var error: (any Error)? { get }
```

## Discussion

The value of this property is `nil` unless the looper’s status changes to AVPlayerLooper.Status.failed. If this occurs, this property value contains an error object that provides the details of the error that prevented looping.


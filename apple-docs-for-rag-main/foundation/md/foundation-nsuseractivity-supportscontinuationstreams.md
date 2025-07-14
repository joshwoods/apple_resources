

- Foundation
- NSUserActivity
-  supportsContinuationStreams 

Instance Property

# supportsContinuationStreams

A Boolean value that determines whether the continuing app can request streams to be opened back to the originating app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var supportsContinuationStreams: Bool { get set }
```

## Discussion

If the value of this property is true, the continuing app can connect back to the originating app for more information using streams. The default value of this property is false. It can dynamically be set to true to selectively support continuation streams based on the state of the user activity.

## See Also

### Working with continuation streams

func getContinuationStreams(completionHandler: (InputStream?, OutputStream?, (any Error)?) -> Void)

Requests streams back to the originating app.




- AVFoundation
- AVCaptureInput
-  ports 

Instance Property

# ports

The ports available on a capture input.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var ports: [AVCaptureInput.Port] { get }
```

## Discussion

Individual ports post an formatDescriptionDidChangeNotification notification when their formatDescription changes.

## See Also

### Accessing Ports

class Port

An object that represents a stream of data that a capture input provides.


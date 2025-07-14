

- AVFoundation
- AVCaptureSession
-  beginConfiguration() 

Instance Method

# beginConfiguration()

Marks the beginning of changes to a running capture session’s configuration to perform in a single atomic update.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func beginConfiguration()
```

## Mentioned in 

Setting Up a Capture Session

## Discussion

Call this method and commitConfiguration() to batch multiple configuration operations on a running session into an atomic update.

After you call this method, you can add or remove outputs, alter the sessionPreset, or configure individual capture input or output properties. The session configuration doesn’t change until you invoke commitConfiguration(), at which the system updates all settings. You can nest beginConfiguration() and commitConfiguration() pairs, and the system applies the changes when you call the outermost commit.

## See Also

### Configuring a Session

func commitConfiguration()

Commits one or more changes to a running capture session’s configuration in a single atomic update.


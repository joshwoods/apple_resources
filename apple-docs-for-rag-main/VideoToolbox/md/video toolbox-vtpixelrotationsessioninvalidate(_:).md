

- Video Toolbox
-  VTPixelRotationSessionInvalidate(\_:) 

Function

# VTPixelRotationSessionInvalidate(\_:)

Tears down a pixel rotation session.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func VTPixelRotationSessionInvalidate(_ session: VTPixelRotationSession)
```

## Parameters 

`session`  

The pixel rotation session to invalidate.

## Discussion

When a pixel rotation session’s retain count reaches zero, the system automatically invalidates it. However, because other processes may retain a session, it can be hard to predict when the invalidation occurs. Calling this function ensures a deterministic, orderly teardown.

## See Also

### Managing a Session

func VTPixelRotationSessionCreate(CFAllocator?, UnsafeMutablePointer&lt;VTPixelRotationSession?>) -> OSStatus

Creates a session to rotate images between pixel buffers.


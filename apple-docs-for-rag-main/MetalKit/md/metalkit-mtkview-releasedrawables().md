

- MetalKit
- MTKView
-  releaseDrawables() 

Instance Method

# releaseDrawables()

Releases the depthStencilTexture and multisampleColorTexture objects.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func releaseDrawables()
```

## Discussion

Call this method when your app is moving to the background or when the view won’t display content for a significant period of time. The texture objects that this class creates consume a large amount of memory, so freeing them makes that memory available to other parts of your app.


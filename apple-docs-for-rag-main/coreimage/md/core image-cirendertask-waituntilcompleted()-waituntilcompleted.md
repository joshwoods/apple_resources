

- Core Image
- CIRenderTask
-  waitUntilCompleted() 

Instance Method

# waitUntilCompleted()

Waits until the CIRenderTask finishes and returns.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func waitUntilCompleted() throws -> CIRenderInfo
```

## Parameters 

`error`  

nil unless the render task failed

## Discussion

Synchronously blocks execution until the CIRenderTask either completes or fails (with error). Calling this method after startTask(toRender:to:) or startTask(toRender:from:to:at:) makes the render task behave synchronously, as if the CPU and GPU were operating as a single unit.


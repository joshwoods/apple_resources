

- Core Image
- CIContext
-  clearCaches() 

Instance Method

# clearCaches()

Frees any cached data, such as temporary images, associated with the context and runs the garbage collector.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.4+tvOS 10.0+visionOS 1.0+

``` source
func clearCaches()
```

## Discussion

You can use this method to remove textures from the texture cache that reference deleted images.

## See Also

### Managing Resources

func reclaimResources()

Runs the garbage collector to reclaim any resources that the context no longer requires.

class func offlineGPUCount() -> UInt32

Returns the number of GPUs not currently driving a display.

var workingColorSpace: CGColorSpace?

The working color space of the Core Image context.

var workingFormat: CIFormat

The working pixel format of the Core Image context.


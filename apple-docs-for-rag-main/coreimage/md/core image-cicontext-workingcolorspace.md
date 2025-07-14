

- Core Image
- CIContext
-  workingColorSpace 

Instance Property

# workingColorSpace

The working color space of the Core Image context.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var workingColorSpace: CGColorSpace? { get }
```

## Discussion

The working color space determines the color space used when executing filter kernels; Core Image automatically converts to and from the source and destination color spaces of input images and output contexts. You specify a working color space using the workingColorSpace key in the `options` dictionary when creating a Core Image context.

## See Also

### Managing Resources

func clearCaches()

Frees any cached data, such as temporary images, associated with the context and runs the garbage collector.

func reclaimResources()

Runs the garbage collector to reclaim any resources that the context no longer requires.

class func offlineGPUCount() -> UInt32

Returns the number of GPUs not currently driving a display.

var workingFormat: CIFormat

The working pixel format of the Core Image context.


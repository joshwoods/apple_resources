

- Core Image
- CIContext
-  workingFormat 

Instance Property

# workingFormat

The working pixel format of the Core Image context.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var workingFormat: CIFormat { get }
```

## Discussion

The working format determines the pixel format that Core Image uses to create intermediate buffers for executing filter kernels. Core Image automatically converts to and from the source and destination pixel formats of input images and output contexts. You specify a working pixel format using the workingFormat key in the `options` dictionary when creating a Core Image context.

## See Also

### Managing Resources

func clearCaches()

Frees any cached data, such as temporary images, associated with the context and runs the garbage collector.

func reclaimResources()

Runs the garbage collector to reclaim any resources that the context no longer requires.

class func offlineGPUCount() -> UInt32

Returns the number of GPUs not currently driving a display.

var workingColorSpace: CGColorSpace?

The working color space of the Core Image context.


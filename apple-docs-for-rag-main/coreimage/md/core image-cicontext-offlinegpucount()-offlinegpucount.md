

- Core Image
- CIContext
-  offlineGPUCount() 

Type Method

# offlineGPUCount()

Returns the number of GPUs not currently driving a display.

macOS 10.10+

``` source
class func offlineGPUCount() -> UInt32
```

## Return Value

The number of offline GPU devices.

## Discussion

If this count is greater than zero, the system has attached GPU devices that are not currently driving a display. You can use these devices for Core Image rendering by creating a context with the init(forOfflineGPUAt:) orinit(forOfflineGPUAt:colorSpace:options:sharedContext:) method.

## See Also

### Managing Resources

func clearCaches()

Frees any cached data, such as temporary images, associated with the context and runs the garbage collector.

func reclaimResources()

Runs the garbage collector to reclaim any resources that the context no longer requires.

var workingColorSpace: CGColorSpace?

The working color space of the Core Image context.

var workingFormat: CIFormat

The working pixel format of the Core Image context.


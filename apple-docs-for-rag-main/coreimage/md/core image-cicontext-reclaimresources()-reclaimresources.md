

- Core Image
- CIContext
-  reclaimResources() 

Instance Method

# reclaimResources()

Runs the garbage collector to reclaim any resources that the context no longer requires.

macOS 10.4+

``` source
func reclaimResources()
```

## Discussion

The system calls this method automatically after every rendering operation. You can use this method to remove textures from the texture cache that reference deleted images.

## See Also

### Managing Resources

func clearCaches()

Frees any cached data, such as temporary images, associated with the context and runs the garbage collector.

class func offlineGPUCount() -> UInt32

Returns the number of GPUs not currently driving a display.

var workingColorSpace: CGColorSpace?

The working color space of the Core Image context.

var workingFormat: CIFormat

The working pixel format of the Core Image context.




- Quartz
- IKSlideshowDataSource
-  slideshowDidStop() 

Instance Method

# slideshowDidStop()

Performs custom tasks when the slideshow stops.

macOS 10.4+

``` source
optional func slideshowDidStop()
```

## Discussion

TImage Kit invokes this method when the slideshow stops. Implement this method to perform custom tasks at that time.

## See Also

### Related Documentation

protocol IKSlideshowDataSource

The `IKSlideshowDataSource` protocol describes the methods that an IKSlideshow object uses to access the contents of its data source object.

### Performing Custom Tasks

func slideshowWillStart()

Performs custom tasks when the slideshow is about to start.

func slideshowDidChangeCurrentIndex(Int)

Performs custom tasks when the slideshow changes to the item at the specified index.


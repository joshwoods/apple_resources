

- Quartz
- IKSlideshowDataSource
-  slideshowWillStart() 

Instance Method

# slideshowWillStart()

Performs custom tasks when the slideshow is about to start.

macOS 10.4+

``` source
optional func slideshowWillStart()
```

## Discussion

Image Kit invokes this method when the slideshow is about to start. Implement this method to perform custom tasks at that time.

## See Also

### Related Documentation

protocol IKSlideshowDataSource

The `IKSlideshowDataSource` protocol describes the methods that an IKSlideshow object uses to access the contents of its data source object.

### Performing Custom Tasks

func slideshowDidStop()

Performs custom tasks when the slideshow stops.

func slideshowDidChangeCurrentIndex(Int)

Performs custom tasks when the slideshow changes to the item at the specified index.


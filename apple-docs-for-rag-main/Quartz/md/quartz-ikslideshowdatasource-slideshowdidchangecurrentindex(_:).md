

- Quartz
- IKSlideshowDataSource
-  slideshowDidChangeCurrentIndex(\_:) 

Instance Method

# slideshowDidChangeCurrentIndex(\_:)

Performs custom tasks when the slideshow changes to the item at the specified index.

macOS 10.4+

``` source
optional func slideshowDidChangeCurrentIndex(_ newIndex: Int)
```

## Parameters 

`newIndex`  

The index of the current item.

## Discussion

Image Kit invokes this method when the slideshow changes to the specified item. Implement this method to perform custom tasks at that time.

## See Also

### Performing Custom Tasks

func slideshowWillStart()

Performs custom tasks when the slideshow is about to start.

func slideshowDidStop()

Performs custom tasks when the slideshow stops.




- Address Book
-  ABCancelLoadingImageDataForTag(\_:) 

Function

# ABCancelLoadingImageDataForTag(\_:)

Cancels an asynchronous fetch of an image for the given tag.

macOS

``` source
func ABCancelLoadingImageDataForTag(_ tag: CFIndex)
```

## Parameters 

`tag`  

Used to track an asynchronous fetch. This parameter should have been returned from a previous call to the ABBeginLoadingImageDataForClient(_:_:_:) function.

## Discussion

Use the ABBeginLoadingImageDataForClient(_:_:_:) function to begin an asynchronous fetch. Implement your callback function to receive the fetched image. Use this function to cancel an asynchronous fetch.

## See Also

### Images

func ABBeginLoadingImageDataForClient(ABPersonRef!, ABImageClientCallback!, UnsafeMutableRawPointer!) -> CFIndex

Starts an asynchronous fetch for image data in all locations, and returns a non-zero tag for tracking.


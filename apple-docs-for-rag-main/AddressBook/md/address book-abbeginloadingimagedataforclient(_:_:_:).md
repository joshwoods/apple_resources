

- Address Book
-  ABBeginLoadingImageDataForClient(\_:\_:\_:) 

Function

# ABBeginLoadingImageDataForClient(\_:\_:\_:)

Starts an asynchronous fetch for image data in all locations, and returns a non-zero tag for tracking.

macOS

``` source
func ABBeginLoadingImageDataForClient(
    _ person: ABPersonRef!,
    _ callback: ABImageClientCallback!,
    _ refcon: UnsafeMutableRawPointer!
) -> CFIndex
```

## Parameters 

`person`  

The person whose image data you wish to fetch.

`callback`  

The function to call when the fetch is completed.

`refcon`  

An untyped pointer to program-defined data that will be passed to the callback.

## Return Value

A non-zero tag for tracking

## Discussion

Use this function to begin an asynchronous fetch. Implement your callback function to receive the fetched image. Use the ABCancelLoadingImageDataForTag(_:) function to cancel an asynchronous fetch.

## See Also

### Images

func ABCancelLoadingImageDataForTag(CFIndex)

Cancels an asynchronous fetch of an image for the given tag.


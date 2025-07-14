

- Address Book
-  ABImageClientCallback 

Type Alias

# ABImageClientCallback

Prototype of a callback function used to notify an application when an asynchronous image fetch is complete.

macOS

``` source
typealias ABImageClientCallback = (CFData?, CFIndex, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`imageData`  

The image data in Quicktime compatible format that was loaded from an asynchronous fetch. `NULL` if the fetch failed.

`tag`  

The tracking number for this fetch that should have been obtained from a previous call to the ABBeginLoadingImageDataForClient(_:_:_:) function.

`info`  

An untyped pointer to program-defined data that was passed to the ABBeginLoadingImageDataForClient(_:_:_:) function.

## Discussion

Use the ABBeginLoadingImageDataForClient(_:_:_:) function to begin an asynchronous fetch, and the ABCancelLoadingImageDataForTag(_:) function to cancel an asynchronous fetch.


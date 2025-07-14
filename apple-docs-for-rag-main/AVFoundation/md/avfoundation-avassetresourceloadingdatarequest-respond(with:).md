

- AVFoundation
- AVAssetResourceLoadingDataRequest
-  respond(with:) 

Instance Method

# respond(with:)

Provides data to the loading request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func respond(with data: Data)
```

## Parameters 

`data`  

An instance of NSData containing some or all of the requested bytes.

## Discussion

This method may be invoked multiple times on the same instance of `AVAssetResourceLoadingDataRequest` to provide the full range of requested data incrementally. Upon each invocation, the value of the currentOffset property is updated to match the amount of data provided.

## See Also

### Providing Data to a Request

var requestedLength: Int

The length, in bytes, of the data requested.

var requestedOffset: Int64

The position within the resource of the first byte requested.

var currentOffset: Int64

The position within the resource of the next byte.

var requestsAllDataToEndOfResource: Bool

A Boolean value that indicates the entire remaining length of the resource from the offest to the end of the resource is being requested.


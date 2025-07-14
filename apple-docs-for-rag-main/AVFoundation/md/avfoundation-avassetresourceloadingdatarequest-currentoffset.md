

- AVFoundation
- AVAssetResourceLoadingDataRequest
-  currentOffset 

Instance Property

# currentOffset

The position within the resource of the next byte.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var currentOffset: Int64 { get }
```

## Discussion

When incrementally loading data you should begin loading at this offset, returning the data by invoking the respond(with:) method. Bytes previous to this value have already been provided.

## See Also

### Providing Data to a Request

func respond(with: Data)

Provides data to the loading request.

var requestedLength: Int

The length, in bytes, of the data requested.

var requestedOffset: Int64

The position within the resource of the first byte requested.

var requestsAllDataToEndOfResource: Bool

A Boolean value that indicates the entire remaining length of the resource from the offest to the end of the resource is being requested.


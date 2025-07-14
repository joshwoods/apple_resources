

- AVFoundation
- AVAssetResourceLoadingDataRequest
-  requestedLength 

Instance Property

# requestedLength

The length, in bytes, of the data requested.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var requestedLength: Int { get }
```

## Discussion

If the content length of the resource is unknown, the sum of the requestedLength and requestedOffset properties may be greater than the actual content length. When this situation occurs, an application must attempt to provide as much of the requested data beginning at the requestedOffset property as the resource contains. The application must then invoke either the AVAssetResourceLoadingRequest instance’s finishLoading() method upon success, or the finishLoading(with:) method if an error is encountered during the loading.

## See Also

### Providing Data to a Request

func respond(with: Data)

Provides data to the loading request.

var requestedOffset: Int64

The position within the resource of the first byte requested.

var currentOffset: Int64

The position within the resource of the next byte.

var requestsAllDataToEndOfResource: Bool

A Boolean value that indicates the entire remaining length of the resource from the offest to the end of the resource is being requested.


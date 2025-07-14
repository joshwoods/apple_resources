

- AVFoundation
- AVAssetResourceLoadingDataRequest
-  requestedOffset 

Instance Property

# requestedOffset

The position within the resource of the first byte requested.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var requestedOffset: Int64 { get }
```

## Discussion

When all of the requested bytes that can be provided have been loaded—including the possible contentInformationRequest data in the AVAssetResourceLoadingRequest instance that contains the receiver—the delegate should respond by invoking finishLoading().

If the `requestedOffset` value is beyond the content length of the resource, the AVAssetResourceLoadingRequest instance is sent a finishLoading() message without any prior invocations of respond(with:).

## See Also

### Providing Data to a Request

func respond(with: Data)

Provides data to the loading request.

var requestedLength: Int

The length, in bytes, of the data requested.

var currentOffset: Int64

The position within the resource of the next byte.

var requestsAllDataToEndOfResource: Bool

A Boolean value that indicates the entire remaining length of the resource from the offest to the end of the resource is being requested.


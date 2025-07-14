

- AVFoundation
- AVMetadataItemValueRequest
-  respond(value:) 

Instance Method

# respond(value:)

Returns the metadata item’s value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func respond(value: any NSCopying & NSObjectProtocol)
```

## Parameters 

`value`  

The value to return for the request.

## Discussion

You call this method to return the metadata item’s value.

## See Also

### Handling the Response

func respond(error: any Error)

Returns an error when the system fails to load the value.

var metadataItem: AVMetadataItem?

The metadata item to request a value for.


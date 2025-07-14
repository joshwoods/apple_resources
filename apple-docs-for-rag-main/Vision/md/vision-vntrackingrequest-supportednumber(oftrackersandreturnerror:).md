

- Vision
- VNTrackingRequest
-  supportedNumber(ofTrackersAndReturnError:) 

Instance Method

# supportedNumber(ofTrackersAndReturnError:)

Returns the maximum number of simultaneous trackers for the request.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func supportedNumber(ofTrackersAndReturnError error: NSErrorPointer) -> Int
```

## Parameters 

`error`  

An error that contains the reason why a failure occurs.

## Return Value

The maximum number of trackers given a combination; or `0` if such combination doesn’t exist.


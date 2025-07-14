

- AVFoundation
- AVAssetReaderOutputCaptionAdaptor
-  captionsNotPresentInPreviousGroups(in:) 

Instance Method

# captionsNotPresentInPreviousGroups(in:)

Returns the set of captions in the caption group that weren’t vended by the adaptor.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func captionsNotPresentInPreviousGroups(in captionGroup: AVCaptionGroup) -> [AVCaption]
```

## Parameters 

`captionGroup`  

The caption group to query.

## Return Value

An array of captions not previously vended by the adaptor, or an empty array if there are none.

## See Also

### Reading Caption Groups

func nextCaptionGroup() -> AVCaptionGroup?

Returns the next caption group.




- AVFoundation
- AVAssetReaderOutputCaptionAdaptor
-  nextCaptionGroup() 

Instance Method

# nextCaptionGroup()

Returns the next caption group.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func nextCaptionGroup() -> AVCaptionGroup?
```

## Return Value

The caption group, or `nil` of there are no more groups.

## See Also

### Reading Caption Groups

func captionsNotPresentInPreviousGroups(in: AVCaptionGroup) -> [AVCaption]

Returns the set of captions in the caption group that weren’t vended by the adaptor.


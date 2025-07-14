

- AVFoundation
- AVCaptionGrouper
-  flushAddedCaptions(upTo:) 

Instance Method

# flushAddedCaptions(upTo:)

Creates caption groups for the captions you enqueue up to the time.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func flushAddedCaptions(upTo upToTime: CMTime) -> [AVCaptionGroup]
```

## Parameters 

`upToTime`  

The time up to which the system flushes the queue.

## Return Value

An array of zero or more caption groups.


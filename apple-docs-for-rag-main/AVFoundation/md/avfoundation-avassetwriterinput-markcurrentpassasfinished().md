

- AVFoundation
- AVAssetWriterInput
-  markCurrentPassAsFinished() 

Instance Method

# markCurrentPassAsFinished()

Tells the input to analyze the appended media to determine whether it can improve the results by reencoding certain segments.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func markCurrentPassAsFinished()
```

## Discussion

When the value of the canPerformMultiplePasses property is true, call this method after you append all of your media data. After the input determines if it warrants performing an additional pass, the value of currentPassDescription changes (typically asynchronously) to describe how to set up for the next pass. Although it’s possible to use key-value observing to determine when the value of currentPassDescription changes, it’s typically more convenient to call the respondToEachPassDescription(on:using:) method to start the work for each pass.

After reappending the media data for all of the time ranges of the new pass, call this method again to determine whether to reappend segments in another pass.

Calling this method effectively cancels any previous invocation of requestMediaDataWhenReady(on:using:), which means that you may call requestMediaDataWhenReady(on:using:) again for each new pass. This method provides a convenient way to consolidate these invocations in your code.

After each pass, you have the option of keeping the most recent results by calling markAsFinished(), instead of this method. If the value of currentPassDescription is `nil` at the beginning of a pass, call markAsFinished() to tell the input to not expect any further media data.

If the value of canPerformMultiplePasses is false, the value of currentPassDescription immediately becomes `nil` after calling this method.

Important

Before calling this method, you must add the input to an asset writer and call the writer’s startWriting() method.

## See Also

### Performing Multiple-Pass Encoding

var canPerformMultiplePasses: Bool

A Boolean value that indicates whether the input may perform multiple passes over appended media data.

var currentPassDescription: AVAssetWriterInputPassDescription?

An object that describes the requirements for the current pass.

class AVAssetWriterInputPassDescription

An object that defines the interface to query for the requirements of the current pass.

var performsMultiPassEncodingIfSupported: Bool

A Boolean value that indicates whether the input attempts to encode the source media data using multiple passes.

func respondToEachPassDescription(on: dispatch_queue_t, using: () -> Void)

Tells the input to invoke a callback whenever it begins a new pass.


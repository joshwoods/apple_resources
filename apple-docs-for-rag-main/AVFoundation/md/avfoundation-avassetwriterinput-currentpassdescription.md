

- AVFoundation
- AVAssetWriterInput
-  currentPassDescription 

Instance Property

# currentPassDescription

An object that describes the requirements for the current pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var currentPassDescription: AVAssetWriterInputPassDescription? { get }
```

## Discussion

If the value of this property is `nil`, call the asset writer input’s markAsFinished() method because there are no more requests to fulfill.

During the first pass, the request contains a single time range value, from zero to positive infinity, that indicates to append all media from the source. This condition is also true when canPerformMultiplePasses is false, in which case the asset writer only performs a single pass.

The value of this property is `nil` before you call startWriting() on the containing asset writer. It transitions to an initial non-`nil` value during the call to startWriting(), and changes only after a call to markCurrentPassAsFinished(). You can use the respondToEachPassDescription(on:using:) to have the system call you at the beginning of each pass.

This property is key-value observable. The system doesn’t notify an observer on a specific thread.

## See Also

### Performing Multiple-Pass Encoding

var canPerformMultiplePasses: Bool

A Boolean value that indicates whether the input may perform multiple passes over appended media data.

class AVAssetWriterInputPassDescription

An object that defines the interface to query for the requirements of the current pass.

func markCurrentPassAsFinished()

Tells the input to analyze the appended media to determine whether it can improve the results by reencoding certain segments.

var performsMultiPassEncodingIfSupported: Bool

A Boolean value that indicates whether the input attempts to encode the source media data using multiple passes.

func respondToEachPassDescription(on: dispatch_queue_t, using: () -> Void)

Tells the input to invoke a callback whenever it begins a new pass.




- AVFoundation
- AVAssetWriterInput
-  canPerformMultiplePasses 

Instance Property

# canPerformMultiplePasses

A Boolean value that indicates whether the input may perform multiple passes over appended media data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var canPerformMultiplePasses: Bool { get }
```

## Discussion

When the value for this property is true, configure your source media data for random access. After appending the media data for the current pass, as specified by the currentPassDescription property, call markCurrentPassAsFinished() so the system can determine whether it needs to perform additional passes. The system may perform only the initial pass if it determines there’s no benefit to performing multiple passes.

When the value for this property is false, your source for media data only needs to support sequential access. In this case, append all of the source media one time and call markAsFinished().

The default value is false. Currently the only way for this property to become true is when the value of performsMultiPassEncodingIfSupported is true. The final value is available after you call startWriting().

This property is key-value observable.

## See Also

### Performing Multiple-Pass Encoding

var currentPassDescription: AVAssetWriterInputPassDescription?

An object that describes the requirements for the current pass.

class AVAssetWriterInputPassDescription

An object that defines the interface to query for the requirements of the current pass.

func markCurrentPassAsFinished()

Tells the input to analyze the appended media to determine whether it can improve the results by reencoding certain segments.

var performsMultiPassEncodingIfSupported: Bool

A Boolean value that indicates whether the input attempts to encode the source media data using multiple passes.

func respondToEachPassDescription(on: dispatch_queue_t, using: () -> Void)

Tells the input to invoke a callback whenever it begins a new pass.


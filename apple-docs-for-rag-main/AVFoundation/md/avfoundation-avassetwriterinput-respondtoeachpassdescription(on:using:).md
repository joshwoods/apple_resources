

- AVFoundation
- AVAssetWriterInput
-  respondToEachPassDescription(on:using:) 

Instance Method

# respondToEachPassDescription(on:using:)

Tells the input to invoke a callback whenever it begins a new pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func respondToEachPassDescription(
    on queue: dispatch_queue_t,
    using block: @escaping () -> Void
)
```

## Parameters 

`queue`  

The queue on which to invoke the callback.

`block`  

A callback the input invokes at the beginning of each pass.

## Discussion

A typical implemementation of the callback block performs the following steps:

1.  Gets the value of the currentPassDescription property and configures media data source accordingly.

2.  Calls the requestMediaDataWhenReady(on:using:) method to begin appending data for the current pass.

After you’ve appended all media data for the current pass, call the markCurrentPassAsFinished() method have the system determine whether to perform another pass. If it performs an additional pass the system invokes the callback to begin the next pass. When it determines that it requires no additional passes, the system invokes the callback one final time so the client can invoke markAsFinished() in response to the value of currentPassDescription becoming `nil`.

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

func markCurrentPassAsFinished()

Tells the input to analyze the appended media to determine whether it can improve the results by reencoding certain segments.

var performsMultiPassEncodingIfSupported: Bool

A Boolean value that indicates whether the input attempts to encode the source media data using multiple passes.


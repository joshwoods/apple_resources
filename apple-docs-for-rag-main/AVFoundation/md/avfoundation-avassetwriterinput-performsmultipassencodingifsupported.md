

- AVFoundation
- AVAssetWriterInput
-  performsMultiPassEncodingIfSupported 

Instance Property

# performsMultiPassEncodingIfSupported

A Boolean value that indicates whether the input attempts to encode the source media data using multiple passes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var performsMultiPassEncodingIfSupported: Bool { get set }
```

## Discussion

An asset writer input may be able to achieve higher quality and lower data rate by performing multiple passes over the source media. It does this by analyzing the media data it appends and reencodes certain segments with different parameters. To perform the reencoding, you must append the media data for the segments again. See the currentPassDescription property and markCurrentPassAsFinished() method for the means by which the input nominates segments to reappend.

When the value of this property is true, the value of isReadyForMoreMediaData for other inputs attached to the same asset writer may be false more often and for longer periods of time. In particular, the value of isReadyForMoreMediaData for inputs that don’t perform multiple passes may start as false after calling the method asset writer’s startWriting() method, and may not change to true until after all multipass inputs complete their final pass.

When the value of this property is true, the input may store data in one or more temporary files before writing compressed samples to the output file. Use the asset writer’s directoryForTemporaryFiles property if you need to specify the location of temporary file writing.

The default value is false, which means that no additional analysis occurs and it doesn’t reencode segments. Not all asset writer input configurations benefit from performing multiple passes over the source media. To determine whether the selected encoder can perform multiple passes, query the value of canPerformMultiplePasses after calling startWriting().

Important

It’s an error to set this property value to true when the value for expectsMediaDataInRealTime is true. It’s also an error for an asset writer to contain inputs with this property set to true when any of its other inputs have a value of true for expectsMediaDataInRealTime.

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

func respondToEachPassDescription(on: dispatch_queue_t, using: () -> Void)

Tells the input to invoke a callback whenever it begins a new pass.


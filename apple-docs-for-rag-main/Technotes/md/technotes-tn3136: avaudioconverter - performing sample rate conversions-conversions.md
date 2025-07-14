

- Technotes
-  TN3136: AVAudioConverter - performing sample rate conversions 

Article

# TN3136: AVAudioConverter - performing sample rate conversions

Use AVAudioConverter to perform sample rate conversions between PCM audio buffers.

## Overview

Using AVAudioConverter to perform sample rate conversions between PCM audio buffers requires making calls to convert(to:error:withInputFrom:). This method takes an instance of AVAudioBuffer, which stores the output of the conversion, as well as a closure that provides instances of AVAudioBuffer to serve as input to the conversion.

Important

The simpler method convert(to:from:) does not require callbacks to convert between PCM audio buffers, but cannot handle sample rate conversions.

When converting between sample rates, the total number of input frames may be hard to predict. One way to cope with variable buffer sizes while providing input to AVAudioConverter is to fill the input buffers on a sample-by-sample basis. This tech note illustrates such a mechanism using a hypothetical SampleProvider protocol that generates one sample at a time.

The Resampler class gathers all of the components necessary for the conversion: the sample provider that conforms to SampleProvider, the AVAudioConverter instance, and the source AVAudioPCMBuffer instance used in the call to convert(to:error:withInputFrom:). While the Resampler class is concerned with providing the output of the sample rate conversion, the SampleProvider implementation is concerned with providing the input.

## Defining a protocol for providing samples

The SampleProvider protocol is an example of how the Resampler class might interface with a provider class that produces audio samples. The protocol requires a single method to achieve this behavior, which returns the next sample in time.

The mechanism used by the conforming provider class to produce audio samples is an implementation detail and therefore omitted. What is important is that an instance of Resampler be able to ask for a number of samples at each conversion operation.

```
/// A protocol that specifies requirements of a type that is capable of producing audio data on a sample-by-sample basis.
protocol SampleProvider {
    /// Returns the next audio sample.
    func getNextSample() -> Float
}
```

The SampleProvider protocol might be implemented by a signal generator, such as the one described in Building a Signal Generator, by a synthesizer or by a circular buffer, for example.

## Creating a resampler

The Resampler class takes the output of a sample provider, resamples it using AVAudioConverter, and copies the result to all channels of an AudioBufferList:

```
/// A class that resamples the audio data furnished by a sample provider.
class Resampler {
    /// The generic class that implements the SampleProvider protocol.
    let sampleProvider: SampleProvider
    /// The converter that performs the resampling.
    let converter: AVAudioConverter
    /// The source audio buffer that stores the samples which will be fed to the converter.
    let sourceBuffer: AVAudioPCMBuffer

    /// Initializes a resampler with a source sample rate, a destination sample rate, and a sample provider.
    init(sourceSampleRate: Double, destinationSampleRate: Double, provider: SampleProvider) {
        self.sampleProvider = provider

        /// Create source and destination formats with the source and destination sample rates.
        let sourceFormat = AVAudioFormat(commonFormat: .pcmFormatFloat32, sampleRate: sourceSampleRate, channels: 1, interleaved: false)
        let destinationFormat = AVAudioFormat(commonFormat: .pcmFormatFloat32, sampleRate: destinationSampleRate, channels: 2, interleaved: false)

        /// Create the converter with the source and destination formats.
        self.converter = AVAudioConverter(from: sourceFormat, to: destinationFormat)

        /// Create the source audio buffer with the source format and enough capacity.
        self.sourceBuffer = AVAudioPCMBuffer(pcmFormat: sourceFormat, frameCapacity: 4096)
    }

    func refill(inNumberOfPackets: AVAudioPacketCount) -> AVAudioPCMBuffer {
        /// See code for this function below.
    }

    func resample(ioData: UnsafeMutablePointer, inNumberFrames: UInt32) {
        /// See code for this function below.
    }
}
```

The converter asks for input buffers in the closure provided to convert(to:error:withInputFrom:). In order to avoid allocating audio buffers every time the converter asks for more input, the Resampler class reuses the source buffer that is passed as input to the converter. The source buffer’s underlying memory is simply refilled with the SampleProvider output for the requested number of frames and returned.

```
/// Takes as input the number of frames to be refilled.
/// Returns an audio buffer that references memory owned by the resampler, after refilling this memory with the output of the sample provider.
func refill(numberOfFrames: AVAudioPacketCount) -> AVAudioPCMBuffer {
    /// Store a pointer to the source buffer sample data.
    let sourceData = sourceBuffer.floatChannelData[0]

    /// Refill the source audio buffer with the requested number of frames.
    for frameIndex in 0..

The AudioBufferList pointer that is provided in the call to `resample(ioData:)` is wrapped in an instance of AVAudioPCMBuffer using the init(pcmFormat:bufferListNoCopy:deallocator:) initializer. This buffer is passed to the converter in the call to convert(to:error:withInputFrom:) to store the output of the conversion. The converter calls the provided closure, passing it the input length and asking for a status flag and a returned audio buffer. The status is always AVAudioConverterInputStatus.haveData in this case, since the sample provider can always produce an arbitrary number of samples. The returned audio buffer is the result of a call to `refill(inNumberOfPackets:)`, using the provided input length.

```
/// Takes as input an AudioBufferList pointer.
/// Resamples the output of the sample provider and copies the result to the given audio buffer list.
func resample(ioData: UnsafeMutablePointer) {
    /// Create the destination audio buffer with the converter output format and referencing the provided AudioBufferList pointer.
    /// The buffers referred to by ioData are provided by the caller to be filled with output samples only and should not contain input samples.
    guard let destinationBuffer = AVAudioPCMBuffer(pcmFormat: converter.outputFormat, bufferListNoCopy: ioData) else { return }
    /// Create a local variable to hold a conversion error.
    var error: NSError?

    /// Perform a conversion operation and store the output in the destination buffer. The provided input will be the returned value of the trailing closure.
    let outputStatus = converter.convert(to: destinationBuffer, error: &error) { [unowned self] numberOfFrames, inputStatus in
        /// Tell the converter there is data available, since a SampleProvider can produce audio data on a sample-by-sample basis.
        inputStatus.pointee = .haveData
        /// Return the refilled source buffer.
        return self.refill(numberOfFrames: numberOfFrames)
    }

    if outputStatus == .error {
        /// If a conversion error occurred, log its localized description.
        if let error = error {
            print(error.localizedDescription)
        }
    }
}
```

The call to convert(to:error:withInputFrom:) attempts to fill the output buffer to its capacity, hence a single call is made to convert(to:error:withInputFrom:) in `resample(ioData:)`. Other conversion scenarios, such as audio data streamed from a file or over a network, or when the conversion involves compressed formats will often involve multiple calls to convert(to:error:withInputFrom:), depending on the returned AVAudioConverterOutputStatus.

## Revision History

- **2023-01-10** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.


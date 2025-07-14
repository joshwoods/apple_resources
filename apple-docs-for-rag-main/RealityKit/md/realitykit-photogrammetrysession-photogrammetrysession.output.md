

- RealityKit
- PhotogrammetrySession
-  PhotogrammetrySession.Output 

Enumeration

# PhotogrammetrySession.Output

Status updates on the object-creation process.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum Output
```

## Mentioned in 

Creating 3D objects from photographs

## Overview

RealityKit’s Object Capture is a long-running background task. The session publishes messages status and error messages to outputs, a Swift AsyncSequence.

Your app can respond to these updates using a `for`-`await`-`in` loop inside of a `Task`, as this example demonstrates.

```
let waiter = Task {
    do {
        for try await output in session.outputs {
            switch output {
                case .processingComplete:
                    // RealityKit has processed all requests.
                case .requestError(let request, let error):
                    // Request encountered an error.
                case .requestComplete(let request, let result):
                    // RealityKit has finished processing a request.
                case .requestProgress(let request, let fractionComplete):
                    // Periodic progress update. Update UI here.
                case requestProgressInfo(let request, let progressInfo):
                    // Periodic progress info update.
                case .inputComplete:
                    // Ingestion of images is complete and processing begins.
                case .invalidSample(let id, let reason):
                    // RealityKit deemed a sample invalid and didn't use it.
                case .skippedSample(let id):
                    // RealityKit was unable to use a provided sample.
                case .automaticDownsampling:
                    // RealityKit downsampled the input images because of
                    // resource constraints.
                case .processingCancelled
                    // Processing was canceled.
                @unknown default:
                    // Unrecognized output.
            }
        }
    } catch {
        print("Output: ERROR = \(String(describing: error))")
        // Handle error.
    }
}

```

## Topics

### Monitoring session status

case inputComplete

The data ingestion portion of the process is complete.

case processingComplete

The session completed a request successfully.

case processingCancelled

All pending requests are canceled.

### Monitoring request status

case requestProgress(PhotogrammetrySession.Request, fractionComplete: Double)

A progress update provided by the session.

case requestComplete(PhotogrammetrySession.Request, PhotogrammetrySession.Result)

The session finished handling all pending requests.

case requestError(PhotogrammetrySession.Request, any Error)

The session aborted a request due to an error.

### Monitoring data ingestion

case invalidSample(id: Int, reason: String)

A provided sample was invalid.

case automaticDownsampling

The session reduced the image size because of memory constraints.

case skippedSample(id: Int)

The type of element used for Object Capture updates. The PhotogrammetrySample with the id indicated was not able to be used for reconstruction.

### Describing updates

var localizedDescription: String

Localized string containing any extra information about the message, such as the reason why a sample is invalid.

### Iterating outputs

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element used for Photogrammetry Session updates.

struct Outputs

An asynchronous sequence of session-related updates.

### Structures

struct ProgressInfo

ProgressInfo includes the estimated remaining time and the progress stage during reconstruction.

### Enumeration Cases

case requestProgressInfo(PhotogrammetrySession.Request, PhotogrammetrySession.Output.ProgressInfo)

case stitchingIncomplete

The session reconstruction could not fully stitch all images of the object.

### Enumerations

enum ProcessingStage

Processing stages during reconstruction.

## See Also

### Monitoring the session

var activeRequests: [PhotogrammetrySession.Request]

The session’s active request objects.

var isProcessing: Bool

The session is actively processing requests.

var outputs: PhotogrammetrySession.Outputs

Returns the outputs message stream which can be asynchronously iterated on.


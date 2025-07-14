

- Sound Analysis
-  SNAudioFileAnalyzer 

Class

# SNAudioFileAnalyzer

An analyzer that runs sound classification requests on an audio file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class SNAudioFileAnalyzer
```

## Mentioned in 

Classifying Sounds in an Audio File

Classifying Sounds in an Audio Stream

## Overview

Run an SNRequest on an audio file by creating an `SNAudioFileAnalyzer`. You can run the same sound analysis request on multiple file analyzers, and each analyzer can process multiple requests. An audio file analyzer generates an SNResult each time any of its active requests recognizes a sound.

## Topics

### Creating an Analyzer

init(url: URL) throws

Creates a new audio file analyzer.

### Managing Requests

func add(any SNRequest, withObserver: any SNResultsObserving) throws

Adds a new analysis request to the audio file analyzer.

protocol SNRequest

A protocol that represents sound analysis requests.

protocol SNResultsObserving

The interface your app implements to receive the results of an analysis request.

func remove(any SNRequest)

Removes an existing request from the audio file analyzer.

func removeAllRequests()

Removes all the sound analysis requests from the audio file analyzer.

### Analyzing Data

func analyze()

Analyzes the audio file synchronously.

func analyze(completionHandler: (Bool) -> Void)

Analyzes the audio file asynchronously.

func cancelAnalysis()

Cancels all the asynchronous sound analysis requests the analyzer is currently processing.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio analyzers

Classifying Sounds in an Audio File

Identify individual sounds in a file, such as a recording, with an audio file analyzer.

Classifying Sounds in an Audio Stream

Identify individual sounds in an audio data stream, such as from a microphone, with an audio stream analyzer.

class SNAudioStreamAnalyzer

An object you create to analyze a stream of audio data and provide the results to your app.


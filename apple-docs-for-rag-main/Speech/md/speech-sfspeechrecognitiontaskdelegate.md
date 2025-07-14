

- Speech
-  SFSpeechRecognitionTaskDelegate 

Protocol

# SFSpeechRecognitionTaskDelegate

A protocol with methods for managing multi-utterance speech recognition requests.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
protocol SFSpeechRecognitionTaskDelegate : NSObjectProtocol
```

## Overview

The methods of this protocol give you fine-grained control over the speech recognition process. Specifically, you use this protocol when you want to know the following:

- When the first utterances of speech occur in the audio.

- When the speech recognizer stops accepting audio.

- When the speech recognition process finishes or is canceled.

- When the speech recognizer generates a potential transcription.

Adopt the methods of this protocol in an object and pass that object in to the `delegate` parameter of recognitionTask(with:delegate:) when starting your speech recognition task.

## Topics

### Tracking the Task Progress

func speechRecognitionDidDetectSpeech(SFSpeechRecognitionTask)

Tells the delegate when the task first detects speech in the source audio.

func speechRecognitionTaskFinishedReadingAudio(SFSpeechRecognitionTask)

Tells the delegate when the task is no longer accepting new audio input, even if final processing is in progress.

### Getting Transcriptions

func speechRecognitionTask(SFSpeechRecognitionTask, didHypothesizeTranscription: SFTranscription)

Tells the delegate that a hypothesized transcription is available.

### Finishing a Speech Recognition Task

func speechRecognitionTask(SFSpeechRecognitionTask, didFinishRecognition: SFSpeechRecognitionResult)

Tells the delegate when the final utterance is recognized.

func speechRecognitionTask(SFSpeechRecognitionTask, didFinishSuccessfully: Bool)

Tells the delegate when the recognition of all requested utterances is finished.

func speechRecognitionTaskWasCancelled(SFSpeechRecognitionTask)

Tells the delegate that the task has been canceled.

### Instance Methods

func speechRecognitionTask(SFSpeechRecognitionTask, didProcessAudioDuration: TimeInterval)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Performing Speech Recognition on Audio

func recognitionTask(with: SFSpeechRecognitionRequest, resultHandler: (SFSpeechRecognitionResult?, (any Error)?) -> Void) -> SFSpeechRecognitionTask

Executes the speech recognition request and delivers the results to the specified handler block.

func recognitionTask(with: SFSpeechRecognitionRequest, delegate: any SFSpeechRecognitionTaskDelegate) -> SFSpeechRecognitionTask

Recognizes speech from the audio source associated with the specified request, using the specified delegate to manage the results.


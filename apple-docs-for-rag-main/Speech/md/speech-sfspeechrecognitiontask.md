

- Speech
-  SFSpeechRecognitionTask 

Class

# SFSpeechRecognitionTask

A task object for monitoring the speech recognition progress.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class SFSpeechRecognitionTask
```

## Overview

Use an `SFSpeechRecognitionTask` object to determine the state of a speech recognition task, to cancel an ongoing task, or to signal the end of the task.

You don’t create speech recognition task objects directly. Instead, you receive one of these objects after calling recognitionTask(with:resultHandler:) or recognitionTask(with:delegate:) on your SFSpeechRecognizer object.

## Topics

### Canceling a Speech Recognition Task

func cancel()

Cancels the current speech recognition task.

var isCancelled: Bool

A Boolean value that indicates whether the speech recognition task was canceled.

### Finishing a Speech Recognition Task

func finish()

Stops accepting new audio and finishes processing on the audio input that has already been accepted.

var isFinishing: Bool

A Boolean value that indicates whether audio input has stopped.

### Monitoring Recognition Progress

var state: SFSpeechRecognitionTaskState

The current state of the speech recognition task.

enum SFSpeechRecognitionTaskState

The state of the task associated with the recognition request.

var error: (any Error)?

An error object that specifies the error that occurred during a speech recognition task.

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


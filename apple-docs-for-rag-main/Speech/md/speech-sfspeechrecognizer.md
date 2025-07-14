

- Speech
-  SFSpeechRecognizer 

Class

# SFSpeechRecognizer

An object you use to check for the availability of the speech recognition service, and to initiate the speech recognition process.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class SFSpeechRecognizer
```

## Mentioned in 

Asking Permission to Use Speech Recognition

## Overview

An SFSpeechRecognizer object is the central object for managing the speech recognizer process. Use this object to:

- Request authorization to use speech recognition services.

- Specify the language to use during the recognition process.

- Initiate new speech recognition tasks.

### Set Up Speech Recognition

Each speech recognizer supports only one language, which you specify at creation time. The successful creation of a speech recognizer does not guarantee that speech recognition services are available. For some languages, the recognizer might require an Internet connection. Use the isAvailable property to find out if speech recognition services are available for the current language.

To initiate the speech recognition process, do the following:

1.  Request authorization to use speech recognition. See Asking Permission to Use Speech Recognition.

2.  Create an SFSpeechRecognizer object.

3.  Verify the availability of services using the isAvailable property of your speech recognizer object.

4.  Prepare your audio content.

5.  Create a recognition request object—an object that descends from SFSpeechRecognitionRequest.

6.  Call the recognitionTask(with:delegate:) or recognitionTask(with:resultHandler:) method to begin the recognition process.

The type of recognition request object you create depends on whether you are processing an existing audio file or an incoming stream of audio. For existing audio files, create a SFSpeechURLRecognitionRequest object. For audio streams, create a SFSpeechAudioBufferRecognitionRequest object.

### Create a Great User Experience for Speech Recognition

Here are some tips to consider when adding speech recognition support to your app.

- **Be prepared to handle failures caused by speech recognition limits.** Because speech recognition is a network-based service, limits are enforced so that the service can remain freely available to all apps. Individual devices may be limited in the number of recognitions that can be performed per day, and each app may be throttled globally based on the number of requests it makes per day. If a recognition request fails quickly (within a second or two of starting), check to see if the recognition service became unavailable. If it is, you may want to ask users to try again later.

- **Plan for a one-minute limit on audio duration.** Speech recognition places a relatively high burden on battery life and network usage. To minimize this burden, the framework stops speech recognition tasks that last longer than one minute. This limit is similar to the one for keyboard-related dictation.

- **Remind the user when your app is recording.** For example, display a visual indicator and play sounds at the beginning and end of speech recognition to help users understand that they’re being actively recorded. You can also display speech as it is being recognized so that users understand what your app is doing and see any mistakes made during the recognition process.

- **Do not perform speech recognition on private or sensitive information.** Some speech is not appropriate for recognition. Don’t send passwords, health or financial data, and other sensitive speech for recognition.

## Topics

### Creating a Speech Recognizer

convenience init?()

Creates a speech recognizer associated with the user’s default language settings.

init?(locale: Locale)

Creates a speech recognizer associated with the specified locale.

### Monitoring the Availability of Speech Recognition

var delegate: (any SFSpeechRecognizerDelegate)?

The delegate object that handles changes to the availability of speech recognition services.

protocol SFSpeechRecognizerDelegate

A protocol that you adopt in your objects to track the availability of a speech recognizer.

var isAvailable: Bool

A Boolean value that indicates whether the speech recognizer is currently available.

var supportsOnDeviceRecognition: Bool

A Boolean value that indicates whether the speech recognizer can operate without network access.

### Requesting Authorization from the User

class func requestAuthorization((SFSpeechRecognizerAuthorizationStatus) -> Void)

Asks the user to allow your app to perform speech recognition.

class func authorizationStatus() -> SFSpeechRecognizerAuthorizationStatus

Returns your app’s current authorization to perform speech recognition.

enum SFSpeechRecognizerAuthorizationStatus

The app’s authorization to perform speech recognition.

### Configuring the Speech Recognizer

var defaultTaskHint: SFSpeechRecognitionTaskHint

A hint that indicates the type of speech recognition being requested.

var queue: OperationQueue

The queue on which to execute recognition task handlers and delegate methods.

### Performing Speech Recognition on Audio

func recognitionTask(with: SFSpeechRecognitionRequest, resultHandler: (SFSpeechRecognitionResult?, (any Error)?) -> Void) -> SFSpeechRecognitionTask

Executes the speech recognition request and delivers the results to the specified handler block.

func recognitionTask(with: SFSpeechRecognitionRequest, delegate: any SFSpeechRecognitionTaskDelegate) -> SFSpeechRecognitionTask

Recognizes speech from the audio source associated with the specified request, using the specified delegate to manage the results.

protocol SFSpeechRecognitionTaskDelegate

A protocol with methods for managing multi-utterance speech recognition requests.

### Getting the Current Language

var locale: Locale

The locale of the speech recognizer.

class func supportedLocales() -> Set&lt;Locale>

Returns the set of locales that are supported by the speech recognizer.

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

### Essentials

Asking Permission to Use Speech Recognition

Ask the user’s permission to perform speech recognition using Apple’s servers.


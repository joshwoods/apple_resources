

- Speech
-  SFSpeechRecognizerDelegate 

Protocol

# SFSpeechRecognizerDelegate

A protocol that you adopt in your objects to track the availability of a speech recognizer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
protocol SFSpeechRecognizerDelegate : NSObjectProtocol
```

## Overview

A speech recognizer’s availability can change due to the device’s Internet connection or other factors. Use this protocol’s optional method to track those changes and provide an appropriate response. For example, when speech recognition becomes unavailable, you might disable related features in your app.

## Topics

### Monitoring the Availability of a Speech Recognizer

func speechRecognizer(SFSpeechRecognizer, availabilityDidChange: Bool)

Tells the delegate that the availability of its associated speech recognizer changed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Monitoring the Availability of Speech Recognition

var delegate: (any SFSpeechRecognizerDelegate)?

The delegate object that handles changes to the availability of speech recognition services.

var isAvailable: Bool

A Boolean value that indicates whether the speech recognizer is currently available.

var supportsOnDeviceRecognition: Bool

A Boolean value that indicates whether the speech recognizer can operate without network access.


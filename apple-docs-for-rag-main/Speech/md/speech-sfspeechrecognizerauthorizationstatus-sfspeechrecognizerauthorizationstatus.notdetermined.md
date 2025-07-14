

- Speech
- SFSpeechRecognizerAuthorizationStatus
-  SFSpeechRecognizerAuthorizationStatus.notDetermined 

Case

# SFSpeechRecognizerAuthorizationStatus.notDetermined

The app’s authorization status has not yet been determined.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
case notDetermined
```

## Discussion

When your app’s status is not determined, calling the requestAuthorization(_:) method prompts the user to grant or deny authorization.

## See Also

### Authorization Statuses

case denied

The user denied your app’s request to perform speech recognition.

case restricted

The device prevents your app from performing speech recognition.

case authorized

The user granted your app’s request to perform speech recognition.


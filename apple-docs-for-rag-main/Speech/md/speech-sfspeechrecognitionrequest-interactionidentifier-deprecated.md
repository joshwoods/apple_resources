

- Speech
- SFSpeechRecognitionRequest
-  interactionIdentifier Deprecated

Instance Property

# interactionIdentifier

An identifier string that you use to describe the type of interaction associated with the speech recognition request.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.15–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var interactionIdentifier: String? { get set }
```

Deprecated

Not used anymore

## Discussion

If different parts of your app have different speech recognition needs, you can use this property to identify the part of your app that is making each request. For example, if one part of your app lets users speak phone numbers and another part lets users speak street addresses, consistently identifying the part of the app that makes a recognition request may help improve the accuracy of the results.


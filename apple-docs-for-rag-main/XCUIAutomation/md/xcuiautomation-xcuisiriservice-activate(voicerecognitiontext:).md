

- XCUIAutomation
- XCUISiriService
-  activate(voiceRecognitionText:) 

Instance Method

# activate(voiceRecognitionText:)

Presents the Siri UI, if it’s not currently active, and accepts a string that is then processed as if it’s recognized speech.

iOS 10.3+iPadOS 10.3+Mac Catalyst 10.3+Xcode 16.3+

``` source
@MainActor
func activate(voiceRecognitionText text: String)
```

## Parameters 

`text`  

The string to pass to Siri for processing.


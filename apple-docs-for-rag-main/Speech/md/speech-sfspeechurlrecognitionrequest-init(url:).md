

- Speech
- SFSpeechURLRecognitionRequest
-  init(url:) 

Initializer

# init(url:)

Creates a speech recognition request, initialized with the specified URL.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
init(url URL: URL)
```

## Discussion

Use this method to create a request to recognize speech in a recorded audio file that resides at the specified URL. Pass the request to the recognizer’s recognitionTask(with:delegate:) method to start recognition.


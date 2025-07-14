

- Speech
- SFSpeechRecognizer
-  recognitionTask(with:resultHandler:) 

Instance Method

# recognitionTask(with:resultHandler:)

Executes the speech recognition request and delivers the results to the specified handler block.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func recognitionTask(
    with request: SFSpeechRecognitionRequest,
    resultHandler: @escaping (SFSpeechRecognitionResult?, (any Error)?) -> Void
) -> SFSpeechRecognitionTask
```

## Parameters 

`request`  

A request (in an SFSpeechRecognitionRequest object) to recognize speech from an audio source.

`resultHandler`  

The block to call when partial or final results are available, or when an error occurs. If the shouldReportPartialResults property is true, this block may be called multiple times to deliver the partial and final results. The block has no return value and takes the following parameters:

result  
A SFSpeechRecognitionResult containing the partial or final transcriptions of the audio content.

error  
An error object if a problem occurred. This parameter is `nil` if speech recognition was successful.

## Return Value

The task object you can use to manage an in-progress recognition request.

## Discussion

Use this method to initiate the speech recognition process on the audio contained in the request object. This method executes asynchronously and returns a SFSpeechRecognitionTask object that you can use to cancel or finalize the recognition process later. As results become available, the method calls the block in the `resultHandler` parameter.

## See Also

### Performing Speech Recognition on Audio

func recognitionTask(with: SFSpeechRecognitionRequest, delegate: any SFSpeechRecognitionTaskDelegate) -> SFSpeechRecognitionTask

Recognizes speech from the audio source associated with the specified request, using the specified delegate to manage the results.

protocol SFSpeechRecognitionTaskDelegate

A protocol with methods for managing multi-utterance speech recognition requests.


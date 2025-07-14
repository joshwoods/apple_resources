

- Sound Analysis
- SNAudioFileAnalyzer
-  cancelAnalysis() 

Instance Method

# cancelAnalysis()

Cancels all the asynchronous sound analysis requests the analyzer is currently processing.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func cancelAnalysis()
```

## Discussion

The method executes asynchronously, and when it completes, the analyzer calls the completion handler you provide to the analyze(completionHandler:) method.

## See Also

### Analyzing Data

func analyze()

Analyzes the audio file synchronously.

func analyze(completionHandler: (Bool) -> Void)

Analyzes the audio file asynchronously.


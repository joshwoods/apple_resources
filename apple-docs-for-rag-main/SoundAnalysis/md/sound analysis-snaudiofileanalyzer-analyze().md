

- Sound Analysis
- SNAudioFileAnalyzer
-  analyze() 

Instance Method

# analyze()

Analyzes the audio file synchronously.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func analyze()
```

## Mentioned in 

Classifying Sounds in an Audio File

## Discussion

This method executes synchronously and may block the calling thread for a long time.

Important

Keep your app’s user interface responsive by calling this method from a thread other than the main thread.

The audio file analyzer sends errors to each request’s results observer.

## See Also

### Analyzing Data

func analyze(completionHandler: (Bool) -> Void)

Analyzes the audio file asynchronously.

func cancelAnalysis()

Cancels all the asynchronous sound analysis requests the analyzer is currently processing.


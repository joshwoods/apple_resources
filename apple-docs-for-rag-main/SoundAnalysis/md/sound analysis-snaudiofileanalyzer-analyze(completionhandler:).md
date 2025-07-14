

- Sound Analysis
- SNAudioFileAnalyzer
-  analyze(completionHandler:) 

Instance Method

# analyze(completionHandler:)

Analyzes the audio file asynchronously.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func analyze(completionHandler: @escaping (Bool) -> Void)
```

``` source
func analyze() async -> Bool
```

## Parameters 

`completionHandler`  

A completion closure (Swift) or block (Objective-C) the analyzer calls when it finishes analyzing a file.

## Mentioned in 

Classifying Sounds in an Audio File

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func analyze() async -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The method executes asynchronously and calls the completion handler after the analyzer finishes analyzing the entire file. The audio file analyzer sends errors to each request’s results observer.

If you call the cancelAnalysis() method, the analyzer calls your completion handler and passes `false` because it can’t reach the end of the file.

## See Also

### Analyzing Data

func analyze()

Analyzes the audio file synchronously.

func cancelAnalysis()

Cancels all the asynchronous sound analysis requests the analyzer is currently processing.


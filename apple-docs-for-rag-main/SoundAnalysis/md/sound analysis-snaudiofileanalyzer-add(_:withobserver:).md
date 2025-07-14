

- Sound Analysis
- SNAudioFileAnalyzer
-  add(\_:withObserver:) 

Instance Method

# add(\_:withObserver:)

Adds a new analysis request to the audio file analyzer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func add(
    _ request: any SNRequest,
    withObserver observer: any SNResultsObserving
) throws
```

## Parameters 

`request`  

A sound analysis request.

`observer`  

An SNResultsObserving instance that receives the analyzer’s results. The analyzer maintains a weak reference to the observer.

## Mentioned in 

Classifying Sounds in an Audio File

## Discussion

The method throws an error (Swift) or returns an error (Objective-C) if the analyzer is actively processing the file.

## See Also

### Managing Requests

protocol SNRequest

A protocol that represents sound analysis requests.

protocol SNResultsObserving

The interface your app implements to receive the results of an analysis request.

func remove(any SNRequest)

Removes an existing request from the audio file analyzer.

func removeAllRequests()

Removes all the sound analysis requests from the audio file analyzer.


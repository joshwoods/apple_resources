

- Sound Analysis
- SNAudioStreamAnalyzer
-  add(\_:withObserver:) 

Instance Method

# add(\_:withObserver:)

Adds a new analysis request to the audio stream analyzer.

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

Classifying Sounds in an Audio Stream

## Discussion

You can add requests to an analyzer that’s actively analyzing an audio stream. The analyzer throws an error (Swift) or returns NO (Objective-C) if it can’t accept the new request, such as a request with an audio format that doesn’t match the analyzer’s.

## See Also

### Managing Requests

protocol SNRequest

A protocol that represents sound analysis requests.

protocol SNResultsObserving

The interface your app implements to receive the results of an analysis request.

func remove(any SNRequest)

Removes an existing request from the audio stream analyzer.

func removeAllRequests()

Removes all the sound analysis requests from the audio stream analyzer.


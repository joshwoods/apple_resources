

- Sound Analysis
- SNAudioStreamAnalyzer
-  removeAllRequests() 

Instance Method

# removeAllRequests()

Removes all the sound analysis requests from the audio stream analyzer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func removeAllRequests()
```

## See Also

### Managing Requests

func add(any SNRequest, withObserver: any SNResultsObserving) throws

Adds a new analysis request to the audio stream analyzer.

protocol SNRequest

A protocol that represents sound analysis requests.

protocol SNResultsObserving

The interface your app implements to receive the results of an analysis request.

func remove(any SNRequest)

Removes an existing request from the audio stream analyzer.


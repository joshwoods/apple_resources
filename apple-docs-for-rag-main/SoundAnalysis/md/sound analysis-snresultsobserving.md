

- Sound Analysis
-  SNResultsObserving 

Protocol

# SNResultsObserving

The interface your app implements to receive the results of an analysis request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol SNResultsObserving : NSObjectProtocol
```

## Mentioned in 

Classifying Sounds in an Audio Stream

Classifying Sounds in an Audio File

## Topics

### Handling Requests

func request(any SNRequest, didProduce: any SNResult)

Provides a new analysis result to your app with the specified time range.

**Required**

protocol SNResult

A protocol that represents sound analysis results.

func request(any SNRequest, didFailWithError: any Error)

Provides any errors that occur during processing of the request.

func requestDidComplete(any SNRequest)

Notifies your app when the analysis request completes normally.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing Requests

func add(any SNRequest, withObserver: any SNResultsObserving) throws

Adds a new analysis request to the audio file analyzer.

protocol SNRequest

A protocol that represents sound analysis requests.

func remove(any SNRequest)

Removes an existing request from the audio file analyzer.

func removeAllRequests()

Removes all the sound analysis requests from the audio file analyzer.


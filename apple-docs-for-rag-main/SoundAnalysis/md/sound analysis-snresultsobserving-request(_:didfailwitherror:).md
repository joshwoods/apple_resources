

- Sound Analysis
- SNResultsObserving
-  request(\_:didFailWithError:) 

Instance Method

# request(\_:didFailWithError:)

Provides any errors that occur during processing of the request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
optional func request(
    _ request: any SNRequest,
    didFailWithError error: any Error
)
```

## Parameters 

`request`  

The request that produces the error.

`error`  

The error that occurs during the request.

## Discussion

The analyzer stops processing a specific request when it encounters an error, and doesn’t call requestDidComplete(_:).

## See Also

### Handling Requests

func request(any SNRequest, didProduce: any SNResult)

Provides a new analysis result to your app with the specified time range.

**Required**

protocol SNResult

A protocol that represents sound analysis results.

func requestDidComplete(any SNRequest)

Notifies your app when the analysis request completes normally.


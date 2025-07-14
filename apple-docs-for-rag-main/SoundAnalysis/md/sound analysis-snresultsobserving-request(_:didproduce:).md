

- Sound Analysis
- SNResultsObserving
-  request(\_:didProduce:) 

Instance Method

# request(\_:didProduce:)

Provides a new analysis result to your app with the specified time range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func request(
    _ request: any SNRequest,
    didProduce result: any SNResult
)
```

**Required**

## Parameters 

`request`  

The request that produces the result.

`result`  

The result of the analysis request.

## Discussion

The analyzer calls this function each time a new analysis result is available. Different types of analyses may produce results at different rates, spanning different time ranges.

## See Also

### Handling Requests

protocol SNResult

A protocol that represents sound analysis results.

func request(any SNRequest, didFailWithError: any Error)

Provides any errors that occur during processing of the request.

func requestDidComplete(any SNRequest)

Notifies your app when the analysis request completes normally.




- Sound Analysis
- SNResultsObserving
-  requestDidComplete(\_:) 

Instance Method

# requestDidComplete(\_:)

Notifies your app when the analysis request completes normally.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
optional func requestDidComplete(_ request: any SNRequest)
```

## Parameters 

`request`  

The request that’s completing.

## Discussion

The analyzer calls this method when it finishes processing the request.

## See Also

### Handling Requests

func request(any SNRequest, didProduce: any SNResult)

Provides a new analysis result to your app with the specified time range.

**Required**

protocol SNResult

A protocol that represents sound analysis results.

func request(any SNRequest, didFailWithError: any Error)

Provides any errors that occur during processing of the request.


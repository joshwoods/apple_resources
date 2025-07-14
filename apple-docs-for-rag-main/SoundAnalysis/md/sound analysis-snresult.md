

- Sound Analysis
-  SNResult 

Protocol

# SNResult

A protocol that represents sound analysis results.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol SNResult : NSObjectProtocol
```

## Overview

Don’t create types that adopt `SNResult`. Only Sound Analysis framework types adopt the protocol.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SNClassificationResult

## See Also

### Handling Requests

func request(any SNRequest, didProduce: any SNResult)

Provides a new analysis result to your app with the specified time range.

**Required**

func request(any SNRequest, didFailWithError: any Error)

Provides any errors that occur during processing of the request.

func requestDidComplete(any SNRequest)

Notifies your app when the analysis request completes normally.


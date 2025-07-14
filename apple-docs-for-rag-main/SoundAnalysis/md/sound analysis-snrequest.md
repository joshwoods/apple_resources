

- Sound Analysis
-  SNRequest 

Protocol

# SNRequest

A protocol that represents sound analysis requests.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol SNRequest : NSObjectProtocol
```

## Overview

Don’t create types that adopt `SNRequest`. Only Sound Analysis framework types adopt the protocol.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- SNClassifySoundRequest

## See Also

### Managing Requests

func add(any SNRequest, withObserver: any SNResultsObserving) throws

Adds a new analysis request to the audio file analyzer.

protocol SNResultsObserving

The interface your app implements to receive the results of an analysis request.

func remove(any SNRequest)

Removes an existing request from the audio file analyzer.

func removeAllRequests()

Removes all the sound analysis requests from the audio file analyzer.


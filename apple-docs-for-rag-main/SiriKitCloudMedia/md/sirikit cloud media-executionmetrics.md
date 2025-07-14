

- SiriKit Cloud Media
-  ExecutionMetrics 

Object

# ExecutionMetrics

Timing information to isolate service performance from network delays.

SiriKit Cloud Media 1.0.2+

``` source
object ExecutionMetrics
```

## Properties

`received`

`date-time`

The UTC time the service receives the request.

`completed`

`date-time`

The UTC time the service finishes processing this Invocation.

`duration`

`float`

The time, in seconds, that elapses while the service processes this request. Provide millisecond precision, if possible.

## See Also

### Instrumenting Your Service

type ServiceDebugReference

A URI that references debugging information for a request.


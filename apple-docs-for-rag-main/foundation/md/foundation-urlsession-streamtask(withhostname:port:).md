

- Foundation
- URLSession
-  streamTask(withHostName:port:) 

Instance Method

# streamTask(withHostName:port:)

Creates a task that establishes a bidirectional TCP/IP connection to a specified hostname and port.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func streamTask(
    withHostName hostname: String,
    port: Int
) -> URLSessionStreamTask
```

## Parameters 

`hostname`  

The hostname of the connection endpoint.

`port`  

The port of the connection endpoint.

## Return Value

The new session stream task.

## Discussion

After you create the task, you must start it by calling its resume() method.

## See Also

### Adding stream tasks to a session

func streamTask(with: NetService) -> URLSessionStreamTask

Creates a task that establishes a bidirectional TCP/IP connection using a specified network service.

Deprecated

class URLSessionStreamTask

A URL session task that is stream-based.

protocol URLSessionStreamDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to stream tasks.




- Foundation
- URLSession
-  streamTask(with:) Deprecated

Instance Method

# streamTask(with:)

Creates a task that establishes a bidirectional TCP/IP connection using a specified network service.

iOS 9.0–18.4DeprecatediPadOS 9.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.11–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func streamTask(with service: NetService) -> URLSessionStreamTask
```

Deprecated

Use nw_connection_t in Network framework instead

## Parameters 

`service`  

A NetService object used to determine the endpoint of the TCP/IP connection. This network service is resolved before any data is read or written to the resulting stream task.

## Return Value

The new session stream task.

## Discussion

After you create the task, you must start it by calling its resume() method.

## See Also

### Adding stream tasks to a session

func streamTask(withHostName: String, port: Int) -> URLSessionStreamTask

Creates a task that establishes a bidirectional TCP/IP connection to a specified hostname and port.

class URLSessionStreamTask

A URL session task that is stream-based.

protocol URLSessionStreamDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events specific to stream tasks.


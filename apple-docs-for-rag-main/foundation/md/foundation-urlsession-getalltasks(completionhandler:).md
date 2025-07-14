

- Foundation
- URLSession
-  getAllTasks(completionHandler:) 

Instance Method

# getAllTasks(completionHandler:)

Asynchronously calls a completion callback with all tasks in a session

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getAllTasks(completionHandler: @escaping ([URLSessionTask]) -> Void)
```

``` source
var allTasks: [URLSessionTask] { get async }
```

## Parameters 

`completionHandler`  

The completion handler to call with the list of tasks.

## See Also

### Managing the session

func finishTasksAndInvalidate()

Invalidates the session, allowing any outstanding tasks to finish.

func flush(completionHandler: () -> Void)

Flushes cookies and credentials to disk, clears transient caches, and ensures that future requests occur on a new TCP connection.

func getTasksWithCompletionHandler(([URLSessionDataTask], [URLSessionUploadTask], [URLSessionDownloadTask]) -> Void)

Asynchronously calls a completion callback with all data, upload, and download tasks in a session.

func invalidateAndCancel()

Cancels all outstanding tasks and then invalidates the session.

func reset(completionHandler: () -> Void)

Empties all cookies, caches and credential stores, removes disk files, flushes in-progress downloads to disk, and ensures that future requests occur on a new socket.

var sessionDescription: String?

An app-defined descriptive label for the session.


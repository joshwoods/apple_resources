

- Foundation
- URLSession
-  invalidateAndCancel() 

Instance Method

# invalidateAndCancel()

Cancels all outstanding tasks and then invalidates the session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func invalidateAndCancel()
```

## Discussion

Once invalidated, references to the delegate and callback objects are broken. After invalidation, session objects cannot be reused.

To allow outstanding tasks to run until completion, call finishTasksAndInvalidate() instead.

Important

Calling this method on the session returned by the shared method has no effect.

## See Also

### Managing the session

func finishTasksAndInvalidate()

Invalidates the session, allowing any outstanding tasks to finish.

func flush(completionHandler: () -> Void)

Flushes cookies and credentials to disk, clears transient caches, and ensures that future requests occur on a new TCP connection.

func getTasksWithCompletionHandler(([URLSessionDataTask], [URLSessionUploadTask], [URLSessionDownloadTask]) -> Void)

Asynchronously calls a completion callback with all data, upload, and download tasks in a session.

func getAllTasks(completionHandler: ([URLSessionTask]) -> Void)

Asynchronously calls a completion callback with all tasks in a session

func reset(completionHandler: () -> Void)

Empties all cookies, caches and credential stores, removes disk files, flushes in-progress downloads to disk, and ensures that future requests occur on a new socket.

var sessionDescription: String?

An app-defined descriptive label for the session.


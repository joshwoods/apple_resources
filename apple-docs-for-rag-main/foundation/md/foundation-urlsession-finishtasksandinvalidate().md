

- Foundation
- URLSession
-  finishTasksAndInvalidate() 

Instance Method

# finishTasksAndInvalidate()

Invalidates the session, allowing any outstanding tasks to finish.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func finishTasksAndInvalidate()
```

## Discussion

This method returns immediately without waiting for tasks to finish. Once a session is invalidated, new tasks cannot be created in the session, but existing tasks continue until completion. After the last task finishes and the session makes the last delegate call related to those tasks, the session calls the urlSession(_:didBecomeInvalidWithError:) method on its delegate, then breaks references to the delegate and callback objects. After invalidation, session objects cannot be reused.

To cancel all outstanding tasks, call invalidateAndCancel() instead.

Important

Calling this method on the session returned by the shared method has no effect.

## See Also

### Managing the session

func flush(completionHandler: () -> Void)

Flushes cookies and credentials to disk, clears transient caches, and ensures that future requests occur on a new TCP connection.

func getTasksWithCompletionHandler(([URLSessionDataTask], [URLSessionUploadTask], [URLSessionDownloadTask]) -> Void)

Asynchronously calls a completion callback with all data, upload, and download tasks in a session.

func getAllTasks(completionHandler: ([URLSessionTask]) -> Void)

Asynchronously calls a completion callback with all tasks in a session

func invalidateAndCancel()

Cancels all outstanding tasks and then invalidates the session.

func reset(completionHandler: () -> Void)

Empties all cookies, caches and credential stores, removes disk files, flushes in-progress downloads to disk, and ensures that future requests occur on a new socket.

var sessionDescription: String?

An app-defined descriptive label for the session.


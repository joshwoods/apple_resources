

- Foundation
-  URLSessionTaskDelegate 

Protocol

# URLSessionTaskDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol URLSessionTaskDelegate : URLSessionDelegate
```

## Mentioned in 

Uploading streams of data

Downloading files from websites

Uploading data to a website

Fetching website data into memory

## Overview

You use this protocol in one of two ways, depending on how you use a URLSession:

- If you create tasks with Swift’s `async`-`await` syntax, using methods like bytes(for:delegate:) and data(for:delegate:), you pass a `delegate` argument of this type. The delegate receives callbacks for things like task progress, while the call point awaits the completion of the task.

- If you add tasks to the session with methods like dataTask(with:) and downloadTask(with:), then you implement this protocol’s methods in a delegate you set on the session. This session delegate may also implement other protocols as appropriate, like URLSessionDownloadDelegate and URLSessionDataDelegate. You can also assign a delegate of this type directly to the task to intercept callbacks before the task delivers them to the session’s delegate.

Note

Your URLSession object doesn’t need to have a delegate. If you don’t assign a delegate, the session uses a system-provided delegate. In this case, you must provide a completion callback or use the Swift `async`-`await` methods to obtain the data.

## Topics

### Handling task life cycle changes

func urlSession(URLSession, task: URLSessionTask, didCompleteWithError: (any Error)?)

Tells the delegate that the task finished transferring data.

### Handling redirects

func urlSession(URLSession, task: URLSessionTask, willPerformHTTPRedirection: HTTPURLResponse, newRequest: URLRequest, completionHandler: (URLRequest?) -> Void)

Tells the delegate that the remote server requested an HTTP redirect.

### Working with upload tasks

func urlSession(URLSession, task: URLSessionTask, didSendBodyData: Int64, totalBytesSent: Int64, totalBytesExpectedToSend: Int64)

Periodically informs the delegate of the progress of sending body content to the server.

func urlSession(URLSession, task: URLSessionTask, needNewBodyStream: (InputStream?) -> Void)

Tells the delegate when a task requires a new request body stream to send to the remote server.

### Handling authentication challenges

func urlSession(URLSession, task: URLSessionTask, didReceive: URLAuthenticationChallenge, completionHandler: (URLSession.AuthChallengeDisposition, URLCredential?) -> Void)

Requests credentials from the delegate in response to an authentication request from the remote server.

enum AuthChallengeDisposition

Constants passed by session or task delegates to the provided continuation block in response to an authentication challenge.

### Handling delayed and waiting tasks

func urlSession(URLSession, task: URLSessionTask, willBeginDelayedRequest: URLRequest, completionHandler: (URLSession.DelayedRequestDisposition, URLRequest?) -> Void)

Tells the delegate that a delayed URL session task will now begin loading.

enum DelayedRequestDisposition

The action to take on a delayed URL session task.

func urlSession(URLSession, taskIsWaitingForConnectivity: URLSessionTask)

Tells the delegate that the task is waiting until suitable connectivity is available before beginning the network load.

### Collecting task metrics

func urlSession(URLSession, task: URLSessionTask, didFinishCollecting: URLSessionTaskMetrics)

Tells the delegate that the session finished collecting metrics for the task.

class URLSessionTaskMetrics

An object encapsulating the metrics for a session task.

### Instance Methods

func urlSession(URLSession, didCreateTask: URLSessionTask)

func urlSession(URLSession, task: URLSessionTask, didReceiveInformationalResponse: HTTPURLResponse)

func urlSession(URLSession, task: URLSessionTask, needNewBodyStreamFrom: Int64, completionHandler: (InputStream?) -> Void)

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable
- URLSessionDelegate

### Inherited By

- URLSessionDataDelegate
- URLSessionDownloadDelegate
- URLSessionStreamDelegate
- URLSessionWebSocketDelegate

## See Also

### Working with a delegate

var delegate: (any URLSessionDelegate)?

The delegate assigned when this object was created.

protocol URLSessionDelegate

A protocol that defines methods that URL session instances call on their delegates to handle session-level events, like session life cycle changes.

var delegateQueue: OperationQueue

The operation queue provided when this object was created.


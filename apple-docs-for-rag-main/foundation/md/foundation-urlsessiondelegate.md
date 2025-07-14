

- Foundation
-  URLSessionDelegate 

Protocol

# URLSessionDelegate

A protocol that defines methods that URL session instances call on their delegates to handle session-level events, like session life cycle changes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol URLSessionDelegate : NSObjectProtocol, Sendable
```

## Mentioned in 

Performing manual server trust authentication

Fetching website data into memory

Downloading files in the background

Uploading data to a website

## Overview

In addition to the methods defined in this protocol, most delegates should also implement some or all of the methods in the URLSessionTaskDelegate, URLSessionDataDelegate, and URLSessionDownloadDelegate protocols to handle task-level events. These include events like the beginning and end of individual tasks, and periodic progress updates from data or download tasks.

Note

Your URLSession object doesn’t need to have a delegate. If no delegate is assigned, a system-provided delegate is used, and you must provide a completion callback to obtain the data.

## Topics

### Handling session life cycle changes

func urlSession(URLSession, didBecomeInvalidWithError: (any Error)?)

Tells the URL session that the session has been invalidated.

func urlSessionDidFinishEvents(forBackgroundURLSession: URLSession)

Tells the delegate that all messages enqueued for a session have been delivered.

### Handling authentication challenges

func urlSession(URLSession, didReceive: URLAuthenticationChallenge, completionHandler: (URLSession.AuthChallengeDisposition, URLCredential?) -> Void)

Requests credentials from the delegate in response to a session-level authentication request from the remote server.

enum AuthChallengeDisposition

Constants passed by session or task delegates to the provided continuation block in response to an authentication challenge.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

### Inherited By

- URLSessionDataDelegate
- URLSessionDownloadDelegate
- URLSessionStreamDelegate
- URLSessionTaskDelegate
- URLSessionWebSocketDelegate

## See Also

### Working with a delegate

var delegate: (any URLSessionDelegate)?

The delegate assigned when this object was created.

protocol URLSessionTaskDelegate

A protocol that defines methods that URL session instances call on their delegates to handle task-level events.

var delegateQueue: OperationQueue

The operation queue provided when this object was created.


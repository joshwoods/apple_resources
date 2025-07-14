

- Foundation
-  NSURLConnectionDelegate 

Protocol

# NSURLConnectionDelegate

A protocol that delegates of a URL connection implement to receive status about and provide feedback to the connection object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSURLConnectionDelegate : NSObjectProtocol
```

## Overview

Delegates of NSURLConnection objects should implement either the NSURLConnectionDataDelegate or NSURLConnectionDownloadDelegate protocol in addition to the NSURLConnectionDelegate protocol. Specifically:

- If you are using NSURLConnection in conjunction with Newsstand Kit’s `download(with:)` method, the delegate class should implement the NSURLConnectionDownloadDelegate protocol.

- Otherwise, the delegate class should implement the NSURLConnectionDataDelegate protocol.

Delegates that wish to perform custom authentication handling should implement the connection(_:willSendRequestFor:) method, which is the preferred mechanism for responding to authentication challenges. (See URLAuthenticationChallenge for more information on authentication challenges.) If connection(_:willSendRequestFor:) is not implemented, the older, deprecated methods connection(_:canAuthenticateAgainstProtectionSpace:), connection(_:didReceive:), and connection(_:didCancel:) are called instead.

The connection(_:didFailWithError:) method is called at most once if an error occurs during the loading of a resource. The connectionShouldUseCredentialStorage(_:) method is called once, just before the loading of a resource begins.

## Topics

### Connection Authentication

func connection(NSURLConnection, willSendRequestFor: URLAuthenticationChallenge)

Tells the delegate that the connection will send a request for an authentication challenge.

func connection(NSURLConnection, canAuthenticateAgainstProtectionSpace: URLProtectionSpace) -> Bool

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

Deprecated

func connection(NSURLConnection, didCancel: URLAuthenticationChallenge)

Sent when a connection cancels an authentication challenge.

Deprecated

func connection(NSURLConnection, didReceive: URLAuthenticationChallenge)

Sent when a connection must authenticate a challenge in order to download its request.

Deprecated

func connectionShouldUseCredentialStorage(NSURLConnection) -> Bool

Sent to determine whether the URL loader should use the credential storage for authenticating the connection.

### Connection Completion

func connection(NSURLConnection, didFailWithError: any Error)

Sent when a connection fails to load its request successfully.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSURLConnectionDataDelegate
- NSURLConnectionDownloadDelegate

## See Also

### URL Connection

class NSURLConnection

An object that enables you to start and stop URL requests.

protocol NSURLConnectionDataDelegate

A protocol that most delegates of a URL connection implement to receive data associated with the connection.

protocol NSURLConnectionDownloadDelegate

A protocol that delegates of a URL connection created with Newsstand Kit implement to receive data associated with a download.




- Foundation
-  URLAuthenticationChallengeSender 

Protocol

# URLAuthenticationChallengeSender

The `URLAuthenticationChallengeSender` protocol represents the interface that the sender of an authentication challenge must implement.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol URLAuthenticationChallengeSender : NSObjectProtocol, Sendable
```

## Overview

The methods in the protocol are generally sent by a delegate in response to receiving a connection(_:didReceive:): or download(_:didReceive:):. The different methods provide different ways of responding to authentication challenges.

Important

This protocol is *only* for use with the legacy NSURLConnection and NSURLDownload classes. It should not be used with URLSession-based code, for which you respond to authentication challenges by passing URLSession.AuthChallengeDisposition constants to the provided completion handler blocks.

## Topics

### Protocol Methods

func cancel(URLAuthenticationChallenge)

Cancels a given authentication challenge.

**Required**

func continueWithoutCredential(for: URLAuthenticationChallenge)

Attempt to continue downloading a request without providing a credential for a given challenge.

**Required**

func use(URLCredential, for: URLAuthenticationChallenge)

Attempt to use a given credential for a given authentication challenge.

**Required**

func performDefaultHandling(for: URLAuthenticationChallenge)

Causes the system-provided default behavior to be used.

func rejectProtectionSpaceAndContinue(with: URLAuthenticationChallenge)

Rejects the currently supplied protection space.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable


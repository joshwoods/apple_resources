

- Foundation
-  URLProtocolClient 

Protocol

# URLProtocolClient

The interface used by URLProtocol subclasses to communicate with the URL Loading System.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol URLProtocolClient : NSObjectProtocol, Sendable
```

## Overview

Don’t implement this protocol in your application. Instead, your URLProtocol subclass calls methods of this protocol on its own client property.

## Topics

### Creating a response

func urlProtocol(URLProtocol, didReceive: URLResponse, cacheStoragePolicy: URLCache.StoragePolicy)

Tells the client that the protocol implementation has created a response object for the request.

**Required**

### Handling redirects

func urlProtocol(URLProtocol, wasRedirectedTo: URLRequest, redirectResponse: URLResponse)

Tells the client that the protocol implementation has been redirected.

**Required**

### Working with cache data

func urlProtocol(URLProtocol, cachedResponseIsValid: CachedURLResponse)

Tells the client that a cached response is valid.

**Required**

### Handling authentication challenges

func urlProtocol(URLProtocol, didCancel: URLAuthenticationChallenge)

Tells the client that an authentication challenge has been canceled.

**Required**

func urlProtocol(URLProtocol, didReceive: URLAuthenticationChallenge)

Tells the client that the URL Loading System received an authentication challenge.

**Required**

### Indicating loading progress or failure

func urlProtocol(URLProtocol, didFailWithError: any Error)

Tells the client that the load request failed due to an error.

**Required**

func urlProtocol(URLProtocol, didLoad: Data)

Tells the client that the protocol implementation has loaded some data.

**Required**

func urlProtocolDidFinishLoading(URLProtocol)

Tells the client that the protocol implementation has finished loading.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Getting protocol attributes

var cachedResponse: CachedURLResponse?

The protocol’s cached response.

var client: (any URLProtocolClient)?

The object the protocol uses to communicate with the URL loading system.

var request: URLRequest

The protocol’s request.

var task: URLSessionTask?

The protocol’s task.




- WebKit
-  WKHTTPCookieStoreObserver 

Protocol

# WKHTTPCookieStoreObserver

The methods to adopt in an object that monitors changes to a webpage’s cookies.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
protocol WKHTTPCookieStoreObserver : NSObjectProtocol
```

## Overview

Adopt the methods of the WKHTTPCookieStoreObserver protocol to track changes to cookies associated with a webpage. To observe the actual cookie changes, call the add(_:) method of the WKHTTPCookieStore you use to manage cookies. When a cookie changes, the cookie store notifies all observers of the changes.

## Topics

### Responding to Cookie Changes

func cookiesDidChange(in: WKHTTPCookieStore)

Tells the delegate that the cookies in the specified cookie store changed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Observing cookie store changes

func add(any WKHTTPCookieStoreObserver)

Adds an observer to the cookie store.

func remove(any WKHTTPCookieStoreObserver)

Removes an observer from the cookie store.




- WebKit
-  WKHTTPCookieStore 

Class

# WKHTTPCookieStore

An object that manages the HTTP cookies associated with a particular web view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
class WKHTTPCookieStore
```

## Overview

Use a WKHTTPCookieStore to specify the initial cookies for your webpages, and to manage cookies for your web content. For example, you might use this object to delete the cookie for the current session when the user logs out. To detect when the webpage changes a cookie, install a cookie observer using the add(_:) method.

You don’t create a WKHTTPCookieStore object directly. Instead, retrieve this object from the WKWebsiteDataStore object in your web view’s configuration object.

## Topics

### Managing cookies

func getAllCookies(([HTTPCookie]) -> Void)

Fetches all stored cookies asynchronously and delivers them to the specified completion handler.

func setCookie(HTTPCookie, completionHandler: (() -> Void)?)

Adds a cookie to the cookie store.

func delete(HTTPCookie, completionHandler: (() -> Void)?)

Deletes the specified cookie.

### Permitting cookie storage

func getCookiePolicy((WKHTTPCookieStore.CookiePolicy) -> Void)

Returns a cookie policy that indicates whether the cookie store allows cookie storage.

func setCookiePolicy(WKHTTPCookieStore.CookiePolicy, completionHandler: (() -> Void)?)

Sets a cookie policy that indicates whether the cookie store allows cookie storage.

enum CookiePolicy

An enumeration with cases that indicate whether a cookie store allows cookie storage.

### Observing cookie store changes

func add(any WKHTTPCookieStoreObserver)

Adds an observer to the cookie store.

func remove(any WKHTTPCookieStoreObserver)

Removes an observer from the cookie store.

protocol WKHTTPCookieStoreObserver

The methods to adopt in an object that monitors changes to a webpage’s cookies.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Web Data Management

class WKWebsiteDataStore

An object that manages cookies, disk and memory caches, and other types of data for a web view.

class WKWebsiteDataRecord

A record of the data that a particular website stores persistently.

protocol WKURLSchemeHandler

A protocol for loading resources with URL schemes that WebKit doesn’t handle.

protocol WKURLSchemeTask

An interface that WebKit uses to request custom resources from your app.

static let readAccessURL: NSAttributedString.DocumentReadingOptionKey

The local files WebKit can access when loading content.


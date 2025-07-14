

- Foundation
-  HTTPCookieStorage 

Class

# HTTPCookieStorage

A container that manages the storage of cookies.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class HTTPCookieStorage
```

## Overview

Each stored cookie is represented by an instance of the HTTPCookie class.

### Sharing cookie storage

The persistent cookie storage returned by shared may be available to app extensions or other apps, subject to the following guidelines:

- iOS — Each app and app extension has a unique data container, meaning they have separate cookie stores. You can obtain a common cookie storage by using the sharedCookieStorage(forGroupContainerIdentifier:) method.

- macOS (non-sandboxed) — As of macOS 10.11, each app has its own cookie storage. Prior to macOS 10.11, a common cookie store is shared among the user’s apps.

- macOS (sandboxed) — Same as iOS.

- UIWebView — `UIWebView` instances within an app inherit the parent app’s shared cookie storage.

- WKWebView — Each `WKWebView` instance has its own cookie storage. See the WKHTTPCookieStore class for more information.

Session cookies (where the cookie object’s isSessionOnly property is true) are local to a single process and are not shared.

Note

In cases where a cookie storage is shared between processes, changes made to the cookie accept policy affect all currently running apps using the cookie storage.

### Subclassing notes

The HTTPCookieStorage class is usable as-is, but you can subclass it. For example, you can override the storage methods like storeCookies(_:for:), getCookiesFor(_:completionHandler:) to screen which cookies are stored, or reimplement the storage mechanism for security or other reasons.

When overriding methods of this class, be aware that methods that take a `task` parameter are preferred by the system to equivalent methods that do not. Therefore, you should override the task-based methods when subclassing, as follows:

- Retrieving cookies — Override getCookiesFor(_:completionHandler:), instead of or in addition to cookies(for:).

- Adding cookies — Override storeCookies(_:for:), instead of or in addition to setCookies(_:for:mainDocumentURL:).

## Topics

### Getting the shared cookie storage object

class var shared: HTTPCookieStorage

The shared cookie storage instance.

class func sharedCookieStorage(forGroupContainerIdentifier: String) -> HTTPCookieStorage

Returns the cookie storage instance for the container associated with the specified app group identifier.

### Getting and setting the cookie accept policy

var cookieAcceptPolicy: HTTPCookie.AcceptPolicy

The cookie storage’s cookie accept policy.

enum AcceptPolicy

Cookie acceptance policies implemented by the HTTPCookieStorage class.

### Adding and removing cookies

func removeCookies(since: Date)

Removes cookies that were stored after a given date.

func deleteCookie(HTTPCookie)

Deletes the specified cookie from the cookie storage.

func setCookie(HTTPCookie)

Stores a specified cookie in the cookie storage if the cookie accept policy permits.

func setCookies([HTTPCookie], for: URL?, mainDocumentURL: URL?)

Adds an array of cookies to the cookie storage if the storage’s cookie acceptance policy permits.

func storeCookies([HTTPCookie], for: URLSessionTask)

Stores an array of cookies in the cookie storage, on behalf of the provided task, if the cookie accept policy permits.

### Retrieving cookies

var cookies: [HTTPCookie]?

The cookie storage’s cookies.

func getCookiesFor(URLSessionTask, completionHandler: ([HTTPCookie]?) -> Void)

Fetches cookies relevant to the specified task and passes them to the completion handler.

func cookies(for: URL) -> [HTTPCookie]?

Returns all the cookie storage’s cookies that are sent to a specified URL.

func sortedCookies(using: [NSSortDescriptor]) -> [HTTPCookie]

Returns all of the cookie storage’s cookies, sorted according to a given set of sort descriptors.

### Tracking cookie storage changes

static let NSHTTPCookieManagerCookiesChanged: NSNotification.Name

A notification posted when the cookies stored in the cookie storage have changed.

static let NSHTTPCookieManagerAcceptPolicyChanged: NSNotification.Name

A notification posted when the acceptance policy of the cookie storage has changed.

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

### Cookies

class HTTPCookie

A representation of an HTTP cookie.


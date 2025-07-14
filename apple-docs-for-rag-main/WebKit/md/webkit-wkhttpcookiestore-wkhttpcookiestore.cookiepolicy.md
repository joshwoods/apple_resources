

- WebKit
- WKHTTPCookieStore
-  WKHTTPCookieStore.CookiePolicy 

Enumeration

# WKHTTPCookieStore.CookiePolicy

An enumeration with cases that indicate whether a cookie store allows cookie storage.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
enum CookiePolicy
```

## Topics

### Specifying a cookie policy

case allow

A case that indicates the cookie store allows cookie storage.

case disallow

A case that indicates the cookie store does not allow cookie storage.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Permitting cookie storage

func getCookiePolicy((WKHTTPCookieStore.CookiePolicy) -> Void)

Returns a cookie policy that indicates whether the cookie store allows cookie storage.

func setCookiePolicy(WKHTTPCookieStore.CookiePolicy, completionHandler: (() -> Void)?)

Sets a cookie policy that indicates whether the cookie store allows cookie storage.




- Foundation
- URL
- URL.FormatStyle
-  init(scheme:user:password:host:port:path:query:fragment:) 

Initializer

# init(scheme:user:password:host:port:path:query:fragment:)

Creates a URL format style with the given display options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    scheme: URL.FormatStyle.ComponentDisplayOption = .always,
    user: URL.FormatStyle.ComponentDisplayOption = .never,
    password: URL.FormatStyle.ComponentDisplayOption = .never,
    host: URL.FormatStyle.HostDisplayOption = .always,
    port: URL.FormatStyle.ComponentDisplayOption = .omitIfHTTPFamily,
    path: URL.FormatStyle.ComponentDisplayOption = .always,
    query: URL.FormatStyle.ComponentDisplayOption = .never,
    fragment: URL.FormatStyle.ComponentDisplayOption = .never
)
```

## Parameters 

`scheme`  

An option to control display of the URL scheme component.

`user`  

An option to control display of the URL user component.

`password`  

An option to control display of the URL password component.

`host`  

An option to control display of the URL host component.

`port`  

An option to control display of the URL port component.

`path`  

An option to control display of the URL path component.

`query`  

An option to control display of the URL query component.

`fragment`  

An option to control display of the URL fragment component.

## Discussion

Explicitly create a URL format style in situations where you want to format multiple URLs with the same style configuration. For one-time use, call formatted() for a default style, or create a style with `URL/FormatStyle/url-4fry3` and customize it with the modifiers in Customizing style behavior.

## See Also

### Creating a URL format style

struct ComponentDisplayOption

A type that indicates whether a formatted URL should include a component.

struct HostDisplayOption

A type that indicates whether a formatted URL should include the host component.


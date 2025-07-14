

- Foundation
- URLComponents
-  url 

Instance Property

# url

A URL created from the components.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var url: URL? { get }
```

## Discussion

If the NSURLComponents has an authority component (user, password, host or port) and a path component, then the path must either begin with “/” or be an empty string. If the NSURLComponents does not have an authority component (user, password, host or port) and has a path component, the path component must not start with “//”. If those requirements are not met, nil is returned.

## See Also

### Getting the URL

func url(relativeTo: URL?) -> URL?

Returns a URL based on the component settings and relative to a given base URL.

var string: String?

A URL derived from the components object, in string form.


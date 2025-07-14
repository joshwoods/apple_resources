

- Foundation
- NSURLComponents
-  url 

Instance Property

# url

A URL object derived from the components object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var url: URL? { get }
```

## Discussion

If the receiver has an authority component (user, password, host, or port) and a path component, then the path must either begin with `"/"` or be an empty string. Otherwise, this property contains `nil`.

If the receiver *does not* have an authority component (user, password, host, or port) and has a path component, the path component must not start with `"//"`. If it does, this property contains `nil`.

If the receiver has `nil` values for all component properties, such as when initializing with init(), this property returns an `NSURL` object with an empty string, because a URL always has a path—even if it’s an empty string.

This property can be used only to obtain a URL based on the values of the other properties. To configure a components object based on an existing URL, call either the componentsWithURL:resolvingAgainstBaseURL: or init(url:resolvingAgainstBaseURL:) method.

## See Also

### Getting the URL

var string: String?

A URL derived from the components object, in string form.

func url(relativeTo: URL?) -> URL?

Returns a URL object derived from the components object.


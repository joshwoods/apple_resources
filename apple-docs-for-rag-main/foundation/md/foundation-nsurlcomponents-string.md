

- Foundation
- NSURLComponents
-  string 

Instance Property

# string

A URL derived from the components object, in string form.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var string: String? { get }
```

## Discussion

If the receiver has an authority component (user, password, host, or port) and a path component, then the path must either begin with `"/"` or be an empty string. Otherwise, this property contains `nil`.

If the receiver *does not* have an authority component (user, password, host, or port) and has a path component, the path component must not start with `"//"`. If it does, this property contains `nil`.

This property can be used only to obtain a URL string based on the values of the other properties. To configure a components object based on an existing URL string, call either the componentsWithString: or init(string:) method.

## See Also

### Getting the URL

var url: URL?

A URL object derived from the components object.

func url(relativeTo: URL?) -> URL?

Returns a URL object derived from the components object.


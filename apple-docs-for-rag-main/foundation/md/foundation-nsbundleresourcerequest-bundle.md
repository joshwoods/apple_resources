

- Foundation
- NSBundleResourceRequest
-  bundle 

Instance Property

# bundle

A reference to the bundle used for storing the downloaded resources. (read-only)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bundle: Bundle { get }
```

## Discussion

This value is either the main bundle or the one specified in the call to init(tags:bundle:). It is valid as soon as the NSBundleResourceRequest object is created.

## See Also

### Accessing the Configuration

var tags: Set&lt;String>

A set of strings, with each string specifying a tag used to mark on-demand resources managed by the request. (read-only)




- WebKit
- WebArchive
-  data Deprecated

Instance Property

# data

The data representation of the receiver.

macOS 10.3–10.14Deprecated

``` source
var data: Data! { get }
```

## Discussion

Can be used to save the web archive to a file, to put it on the pasteboard using the WebArchivePboardType type, or used to initialize another web archive using the init(data:) method.

## See Also

### Getting attributes

var mainResource: WebResource!

The receiver’s main resource.

Deprecated

var subresources: [Any]!

The receiver’s subresources, or `nil` if there are none.

Deprecated

var subframeArchives: [Any]!

Archives representing the receiver’s subresources or `nil` if there are none.

Deprecated


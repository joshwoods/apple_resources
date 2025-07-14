

- Safari Services
- SFUniversalLink
-  applicationURL 

Instance Property

# applicationURL

The URL to the app that can open this universal link.

macOS 10.15+

``` source
var applicationURL: URL { get }
```

## Discussion

The URL represents a location on the file system. You can retrieve additional information about this app using resourceValues(forKeys:).

## See Also

### Configuring Universal Links

var isEnabled: Bool

A flag that indicates whether the universal link is enabled.

var webpageURL: URL

The URL specified when initializing the receiver.


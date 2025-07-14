

- AppKit
- NSSharingService
-  menuItemTitle 

Instance Property

# menuItemTitle

The title of the service in the Share menu.

macOS 10.9+

``` source
var menuItemTitle: String { get set }
```

## Discussion

By default, this title is the same as the value of the title property. Your app can modify this value.

## See Also

### Configuring the Service

var recipients: [String]?

An array containing the user handles of the desired recipients.

var subject: String?

The subject of the post.




- AppKit
- NSSharingService
-  recipients 

Instance Property

# recipients

An array containing the user handles of the desired recipients.

macOS 10.9+

``` source
var recipients: [String]? { get set }
```

## Discussion

Each object in the array is an `NSString` object that contains the handle of a single recipient. The specific format of these handle varies from service to service. For example, some services use email addresses as handles.

## See Also

### Configuring the Service

var menuItemTitle: String

The title of the service in the Share menu.

var subject: String?

The subject of the post.


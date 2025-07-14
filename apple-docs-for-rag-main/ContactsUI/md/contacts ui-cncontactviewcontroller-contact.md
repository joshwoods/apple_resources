

- Contacts UI
- CNContactViewController
-  contact 

Instance Property

# contact

The contact being displayed.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
@MainActor
var contact: CNContact { get }
```

**macOS**

``` source
@NSCopying @MainActor
var contact: CNContact? { get set }
```

## See Also

### Displaying Contact Properties

var alternateName: String?

The name to use if the contact has no display name.

var message: String?

The message displayed under the name of the contact.

var displayedPropertyKeys: [Any]?

The contact property keys to display.


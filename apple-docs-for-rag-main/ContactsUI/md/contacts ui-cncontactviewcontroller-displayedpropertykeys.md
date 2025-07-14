

- Contacts UI
- CNContactViewController
-  displayedPropertyKeys 

Instance Property

# displayedPropertyKeys

The contact property keys to display.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var displayedPropertyKeys: [Any]? { get set }
```

## Discussion

If this property is not set, the view controller displays all properties.

## See Also

### Displaying Contact Properties

var contact: CNContact

The contact being displayed.

var alternateName: String?

The name to use if the contact has no display name.

var message: String?

The message displayed under the name of the contact.


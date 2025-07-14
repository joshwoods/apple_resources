

- Contacts UI
- CNContactViewController
-  parentContainer 

Instance Property

# parentContainer

The container in which to add a new contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var parentContainer: CNContainer? { get set }
```

## Discussion

If you do not set this property, the view controller adds a new contact to the default container.

## See Also

### Configuring the Contact’s Relationships

var parentGroup: CNGroup?

The group in which to add a new contact.


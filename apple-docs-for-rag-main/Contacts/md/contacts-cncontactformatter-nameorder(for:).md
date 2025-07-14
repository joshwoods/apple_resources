

- Contacts
- CNContactFormatter
-  nameOrder(for:) 

Type Method

# nameOrder(for:)

Returns the display name order.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func nameOrder(for contact: CNContact) -> CNContactDisplayNameOrder
```

## Parameters 

`contact`  

The contact whose name is to be formatted.

## Return Value

The display order to use when combining the given name and family name components.

## Discussion

For more information about display name orders, see CNContactDisplayNameOrder.

## See Also

### Getting format information

class func delimiter(for: CNContact) -> String

Returns the delimiter to use between name components.

enum CNContactDisplayNameOrder

The formatting orders for contact names component.


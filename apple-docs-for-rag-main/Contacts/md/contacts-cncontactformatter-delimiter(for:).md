

- Contacts
- CNContactFormatter
-  delimiter(for:) 

Type Method

# delimiter(for:)

Returns the delimiter to use between name components.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func delimiter(for contact: CNContact) -> String
```

## Parameters 

`contact`  

The contact whose name is to be formatted.

## Return Value

The delimiter to use between name components.

## Discussion

If `contact` is `nil`, or if it has no first name, middle name, or last name, this method returns an empty string.

## See Also

### Getting format information

class func nameOrder(for: CNContact) -> CNContactDisplayNameOrder

Returns the display name order.

enum CNContactDisplayNameOrder

The formatting orders for contact names component.


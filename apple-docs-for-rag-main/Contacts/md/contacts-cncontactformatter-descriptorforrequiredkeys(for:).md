

- Contacts
- CNContactFormatter
-  descriptorForRequiredKeys(for:) 

Type Method

# descriptorForRequiredKeys(for:)

Returns the required key descriptor for the specified formatting style of the contact.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func descriptorForRequiredKeys(for style: CNContactFormatterStyle) -> any CNKeyDescriptor
```

## Parameters 

`style`  

The formatting style to be used for contact name.

## Return Value

The contact key descriptor for the formatting style.

## Discussion

Include this method with the keys to fetch when fetching contacts. To format multiple styles, you can include multiple key descriptors with the keys to fetch.

## See Also

### Getting a descriptor

class var descriptorForRequiredKeysForDelimiter: any CNKeyDescriptor

Returns the required key descriptor for the name delimiter.

class var descriptorForRequiredKeysForNameOrder: any CNKeyDescriptor

Returns the required key descriptor for the display name order.


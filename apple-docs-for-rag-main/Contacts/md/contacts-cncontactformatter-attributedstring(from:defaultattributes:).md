

- Contacts
- CNContactFormatter
-  attributedString(from:defaultAttributes:) 

Instance Method

# attributedString(from:defaultAttributes:)

Formats the contact name as an attributed string.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func attributedString(
    from contact: CNContact,
    defaultAttributes attributes: [AnyHashable : Any]? = nil
) -> NSAttributedString?
```

## Parameters 

`contact`  

The contact whose name is to be formatted.

`attributes`  

The default attributes to use. For more information, see Formatter.

## Return Value

The formatted contact name as an attributed string.

## Discussion

This method behaves similarly to string(from:style:), except that it returns an attributed string. It includes the attribute key CNContactPropertyAttribute whose attribute values are contact property keys, such as CNContactGivenNameKey. This identifies the name components in the formatted contact name.

## See Also

### Creating a formatted attributed string

class func attributedString(from: CNContact, style: CNContactFormatterStyle, defaultAttributes: [AnyHashable : Any]?) -> NSAttributedString?

Formats the contact name as an attributed string.


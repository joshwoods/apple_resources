

- Contacts
- CNContactFormatter
-  string(from:style:) 

Type Method

# string(from:style:)

Returns the contact name, formatted with the specified formatter.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class func string(
    from contact: CNContact,
    style: CNContactFormatterStyle
) -> String?
```

## Parameters 

`contact`  

The contact whose name is to be formatted.

`style`  

The formatting style to be used for the contact name.

## Return Value

The formatted contact name.

## See Also

### Creating a formatted string

func string(from: CNContact) -> String?

Formats the contact name.


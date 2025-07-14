

- Contacts
- CNContactFormatter
-  string(from:) 

Instance Method

# string(from:)

Formats the contact name.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func string(from contact: CNContact) -> String?
```

## Parameters 

`contact`  

The contact whose name is to be formatted.

## Return Value

The formatted contact name.

## See Also

### Creating a formatted string

class func string(from: CNContact, style: CNContactFormatterStyle) -> String?

Returns the contact name, formatted with the specified formatter.


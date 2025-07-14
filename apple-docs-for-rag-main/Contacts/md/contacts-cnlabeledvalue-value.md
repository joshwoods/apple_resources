

- Contacts
- CNLabeledValue
-  value 

Instance Property

# value

A contact property value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var value: ValueType { get }
```

## Discussion

A contact property value, such as CNPhoneNumber for a phone number, NSString for an email address, and so on. For valid values, see CNContact properties that are arrays of labeled value objects.

## See Also

### Getting the label and value

var label: String?

The label for a contact property value.


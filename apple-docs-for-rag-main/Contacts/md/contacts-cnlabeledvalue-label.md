

- Contacts
- CNLabeledValue
-  label 

Instance Property

# label

The label for a contact property value.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var label: String? { get }
```

## Discussion

A contact property can have a label, such as Home, Work, iPhone, etc. For some predefined label constants, seeCNPhoneNumber, and CNContactRelation. Custom labels can also be used. Labels are not used for CNSocialProfile and CNInstantMessageAddress properties.

## See Also

### Getting the label and value

var value: ValueType

A contact property value.


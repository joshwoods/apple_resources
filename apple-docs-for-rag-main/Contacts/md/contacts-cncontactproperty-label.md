

- Contacts
- CNContactProperty
-  label 

Instance Property

# label

The label of the labeled value of the property array.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var label: String? { get }
```

## Discussion

Labeled property is used only for properties that are in labeled arrays. If the property is not an array of labeled values, the value of the label is `nil`.

## See Also

### Getting the Property Information

var key: String

The key of the contact property.

var value: Any?

The value of the property.

var identifier: String?

The identifier of the labeled value in the array of labeled.


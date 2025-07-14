

- Contacts
- CNContactProperty
-  identifier 

Instance Property

# identifier

The identifier of the labeled value in the array of labeled.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
var identifier: String? { get }
```

## Discussion

Identifier is used only for properties in labeled arrays. If the property is not an array of labeled values, the value of the identifier is `nil`.

## See Also

### Getting the Property Information

var key: String

The key of the contact property.

var value: Any?

The value of the property.

var label: String?

The label of the labeled value of the property array.


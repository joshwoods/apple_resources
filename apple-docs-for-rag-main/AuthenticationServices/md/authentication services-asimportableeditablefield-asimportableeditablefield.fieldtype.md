

- Authentication Services
- ASImportableEditableField
-  ASImportableEditableField.FieldType 

Enumeration

# ASImportableEditableField.FieldType

An enumeration of editable field types.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
enum FieldType
```

## Topics

### Determining field type

case boolean

A type for a Boolean value field.

case concealedString

A type for a concealed string field.

case date

A type for a date field.

case email

A type for an email field.

case number

A type for a number field.

case string

A type for a concealed string field.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing field properties

var id: Data

A unique identifier for this editable field.

var fieldType: ASImportableEditableField.FieldType

The type of this editable field.

var value: String

The value stored in this editable field.

var label: String?

A value describing the field, if any.


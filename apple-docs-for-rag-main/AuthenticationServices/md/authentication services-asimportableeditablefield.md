

- Authentication Services
-  ASImportableEditableField 

Structure

# ASImportableEditableField

A field that someone can edit within a credential.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
struct ASImportableEditableField
```

## Overview

Examples of editable fields include username and password in ASImportableCredential.BasicAuthentication.

This type is a representation of `EditableField` as defined in the Credential Exchange Format (CXF) specification. You can supply a JSON representation of a CXF `EditableField` to initialize an instance of this struct by using a JSONDecoder and calling decode(_:from:).

## Topics

### Creating an editable field

init(id: Data, fieldType: ASImportableEditableField.FieldType, value: String, label: String?)

Creates an editable field instance.

### Accessing field properties

var id: Data

A unique identifier for this editable field.

var fieldType: ASImportableEditableField.FieldType

The type of this editable field.

enum FieldType

An enumeration of editable field types.

var value: String

The value stored in this editable field.

var label: String?

A value describing the field, if any.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Accessing authentication properties

var urls: [String]

The list of URLs for which to fill the password.

var username: ASImportableEditableField?

The username associated with the credential.

var password: ASImportableEditableField?

The password associated with the credential.


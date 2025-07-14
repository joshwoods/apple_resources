

- Contacts
- CNLabeledValue
-  init(label:value:) 

Initializer

# init(label:value:)

Returns a new labeled value identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
init(
    label: String?,
    value: ValueType
)
```

## Parameters 

`label`  

A string value for the label portion of the object, or `nil` if the value doesn’t have a label.

`value`  

A value for the labeled value object. For valid values, see CNContact properties that are arrays of labeled value objects.

## Return Value

A new labeled value object.


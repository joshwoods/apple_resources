

- Contacts
- CNLabeledValue
-  settingLabel(\_:value:) 

Instance Method

# settingLabel(\_:value:)

Returns a labeled value object with the specified label and value with the existing identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func settingLabel(
    _ label: String?,
    value: ValueType
) -> Self
```

## Parameters 

`label`  

The label of the copied labeled value object, or `nil` if the contact property value doesn’t have a label.

`value`  

The copied labeled value object. For valid values, see CNContact properties that are arrays of labeled value objects.

## Return Value

A labeled value object with the existing identifier.

## See Also

### Setting labels and values

func settingLabel(String?) -> Self

Returns a labeled value object with an existing value and identifier.

func settingValue(ValueType) -> Self

Returns a new value for an existing label and identifier.


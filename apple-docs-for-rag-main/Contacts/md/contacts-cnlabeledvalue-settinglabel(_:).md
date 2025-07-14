

- Contacts
- CNLabeledValue
-  settingLabel(\_:) 

Instance Method

# settingLabel(\_:)

Returns a labeled value object with an existing value and identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func settingLabel(_ label: String?) -> Self
```

## Parameters 

`label`  

The label of the copied labeled value object, or `nil` if the contact property value doesn’t have a label.

## Return Value

A labeled value object with an existing value and identifier.

## See Also

### Setting labels and values

func settingLabel(String?, value: ValueType) -> Self

Returns a labeled value object with the specified label and value with the existing identifier.

func settingValue(ValueType) -> Self

Returns a new value for an existing label and identifier.


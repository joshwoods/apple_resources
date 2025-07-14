

- Contacts
- CNLabeledValue
-  settingValue(\_:) 

Instance Method

# settingValue(\_:)

Returns a new value for an existing label and identifier.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
func settingValue(_ value: ValueType) -> Self
```

## Parameters 

`value`  

A new value for the copied labeled value object. For valid values, see CNContact properties that are arrays of labeled value objects.

## Return Value

The CNLabeledValue object with an existing label and identifier.

## See Also

### Setting labels and values

func settingLabel(String?) -> Self

Returns a labeled value object with an existing value and identifier.

func settingLabel(String?, value: ValueType) -> Self

Returns a labeled value object with the specified label and value with the existing identifier.


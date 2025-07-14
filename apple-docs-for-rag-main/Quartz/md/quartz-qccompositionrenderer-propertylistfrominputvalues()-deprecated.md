

- Quartz
- QCCompositionRenderer
-  propertyListFromInputValues() Deprecated

Instance Method

# propertyListFromInputValues()

Returns a property list object that represents the current values for all the input keys of the composition.

macOS 10.4–10.15Deprecated

``` source
func propertyListFromInputValues() -> Any!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

A property list object.

## Discussion

This is a convenience method that allows you to easily save the set of input values on a composition. Typically, you store the set of values in application preferences.

## See Also

### Saving and Restoring Input Values

func setInputValuesWithPropertyList(Any!)

Sets the values for the input keys of the composition from a previously saved property list.

**Required**

Deprecated


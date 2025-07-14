

- Quartz
- QCCompositionRenderer
-  setInputValuesWithPropertyList(\_:) Deprecated

Instance Method

# setInputValuesWithPropertyList(\_:)

Sets the values for the input keys of the composition from a previously saved property list.

macOS 10.4–10.15Deprecated

``` source
func setInputValuesWithPropertyList(_ plist: Any!)
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Discussion

This is a convenience method that allows you to restore the set of input values that you obtained previously by calling the method propertyListFromInputValues(). If the property list object does not define a value for an input key, or if the value is not of the proper type, Quartz Composer does not set a value for the corresponding input port.

## See Also

### Saving and Restoring Input Values

func propertyListFromInputValues() -> Any!

Returns a property list object that represents the current values for all the input keys of the composition.

**Required**

Deprecated


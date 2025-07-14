

- Quartz
- QCCompositionRenderer
-  setValue(\_:forInputKey:) Deprecated

Instance Method

# setValue(\_:forInputKey:)

Sets the value for an input port of a composition.

macOS 10.4–10.15Deprecated

``` source
func setValue(
    _ value: Any!,
    forInputKey key: String!
) -> Bool
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`value`  

The value to set for the input port. The input port must be at the root patch of the composition. The data type of the `value` argument must match the input port. See QCPortAttributeTypeKey for the data types accepted by a particular port type.

`key`  

The key associated with the input port of the composition. This method throws an exception if `key` is invalid.

## Return Value

Returns false if it cannot set the value.

## See Also

### Passing and Retrieving Values From a Composition

func value(forInputKey: String!) -> Any!

Returns the value for an input port of a composition.

**Required**

Deprecated

func value(forOutputKey: String!) -> Any!

Returns the value for an output port of a composition.

**Required**

Deprecated

func value(forOutputKey: String!, ofType: String!) -> Any!

Returns the current value on an output port (identified by its key) of the root patch of the composition.

**Required**

Deprecated


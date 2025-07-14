

- Quartz
- QCCompositionRenderer
-  value(forInputKey:) Deprecated

Instance Method

# value(forInputKey:)

Returns the value for an input port of a composition.

macOS 10.4–10.15Deprecated

``` source
func value(forInputKey key: String!) -> Any!
```

**Required**

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`key`  

The key associated with an input port for the root patch of a composition. This method throws an exception if `key` is invalid.

## Return Value

The value. The data type of returned value depends on the type of the input port. See QCPortAttributeTypeKey for more information.

## See Also

### Passing and Retrieving Values From a Composition

func setValue(Any!, forInputKey: String!) -> Bool

Sets the value for an input port of a composition.

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


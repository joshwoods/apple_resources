

- Core Media I/O
- CMIOExtensionStreamSource
-  streamProperties(forProperties:) 

Instance Method

# streamProperties(forProperties:)

Gets the states of specified properties.

Mac Catalyst 15.4+macOS 12.3+

``` source
func streamProperties(forProperties properties: Set) throws -> CMIOExtensionStreamProperties
```

**Required**

## Parameters 

`properties`  

A set of properties with states to retrieve.

## Return Value

An object that contains the states of the requested properties.

## See Also

### Managing Stream Properties

var availableProperties: Set&lt;CMIOExtensionProperty>

A set of properties available for the stream.

**Required**

func setStreamProperties(CMIOExtensionStreamProperties) throws

Sets the property state of a stream.

**Required**


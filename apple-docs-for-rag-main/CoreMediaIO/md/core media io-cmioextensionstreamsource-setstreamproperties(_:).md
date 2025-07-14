

- Core Media I/O
- CMIOExtensionStreamSource
-  setStreamProperties(\_:) 

Instance Method

# setStreamProperties(\_:)

Sets the property state of a stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
func setStreamProperties(_ streamProperties: CMIOExtensionStreamProperties) throws
```

**Required**

## Parameters 

`streamProperties`  

A properties object that contains the new property states.

## See Also

### Managing Stream Properties

var availableProperties: Set&lt;CMIOExtensionProperty>

A set of properties available for the stream.

**Required**

func streamProperties(forProperties: Set&lt;CMIOExtensionProperty>) throws -> CMIOExtensionStreamProperties

Gets the states of specified properties.

**Required**


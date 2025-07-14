

- Core Media I/O
- CMIOExtensionStreamSource
-  availableProperties 

Instance Property

# availableProperties

A set of properties available for the stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
var availableProperties: Set { get }
```

**Required**

## See Also

### Managing Stream Properties

func streamProperties(forProperties: Set&lt;CMIOExtensionProperty>) throws -> CMIOExtensionStreamProperties

Gets the states of specified properties.

**Required**

func setStreamProperties(CMIOExtensionStreamProperties) throws

Sets the property state of a stream.

**Required**


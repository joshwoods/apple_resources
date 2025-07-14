

- Core Media I/O
- CMIOExtensionStreamSource
-  formats 

Instance Property

# formats

An array of formats that a stream supports.

Mac Catalyst 15.4+macOS 12.3+

``` source
var formats: [CMIOExtensionStreamFormat] { get }
```

**Required**

## Discussion

Don’t change stream formats during the life cycle of the associated stream.

## See Also

### Accessing the Source Format

class CMIOExtensionStreamFormat

An object that describes the format of a media stream.


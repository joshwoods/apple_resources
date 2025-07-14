

- Latent Semantic Mapping
-  LSMMapWriteToStream(\_:\_:\_:\_:) 

Function

# LSMMapWriteToStream(\_:\_:\_:\_:)

Writes information about a map or text to a stream in text form.

Mac CatalystmacOS

``` source
func LSMMapWriteToStream(
    _ mapref: LSMMap,
    _ textref: LSMText?,
    _ stream: CFWriteStream,
    _ options: CFOptionFlags
) -> OSStatus
```

## See Also

### Loading and Saving a Map

func LSMMapCreateFromURL(CFAllocator?, CFURL, CFOptionFlags) -> Unmanaged&lt;LSMMap>?

Loads a map from the specified file.

func LSMMapWriteToURL(LSMMap, CFURL, CFOptionFlags) -> OSStatus

Compiles the map, if necessary, and stores it into the specified file.

Storage Flags

Options for loading and saving a map to a file.


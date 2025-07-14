

- Latent Semantic Mapping
-  LSMMapWriteToURL(\_:\_:\_:) 

Function

# LSMMapWriteToURL(\_:\_:\_:)

Compiles the map, if necessary, and stores it into the specified file.

Mac CatalystmacOS

``` source
func LSMMapWriteToURL(
    _ mapref: LSMMap,
    _ file: CFURL,
    _ flags: CFOptionFlags
) -> OSStatus
```

## See Also

### Loading and Saving a Map

func LSMMapCreateFromURL(CFAllocator?, CFURL, CFOptionFlags) -> Unmanaged&lt;LSMMap>?

Loads a map from the specified file.

func LSMMapWriteToStream(LSMMap, LSMText?, CFWriteStream, CFOptionFlags) -> OSStatus

Writes information about a map or text to a stream in text form.

Storage Flags

Options for loading and saving a map to a file.


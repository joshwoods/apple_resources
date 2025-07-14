

- Latent Semantic Mapping
-  LSMMapCreateFromURL(\_:\_:\_:) 

Function

# LSMMapCreateFromURL(\_:\_:\_:)

Loads a map from the specified file.

Mac CatalystmacOS

``` source
func LSMMapCreateFromURL(
    _ alloc: CFAllocator?,
    _ file: CFURL,
    _ flags: CFOptionFlags
) -> Unmanaged?
```

## See Also

### Loading and Saving a Map

func LSMMapWriteToURL(LSMMap, CFURL, CFOptionFlags) -> OSStatus

Compiles the map, if necessary, and stores it into the specified file.

func LSMMapWriteToStream(LSMMap, LSMText?, CFWriteStream, CFOptionFlags) -> OSStatus

Writes information about a map or text to a stream in text form.

Storage Flags

Options for loading and saving a map to a file.


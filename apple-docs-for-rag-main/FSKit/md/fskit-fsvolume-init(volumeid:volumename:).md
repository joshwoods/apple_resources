

- FSKit
- FSVolume
-  init(volumeID:volumeName:) 

Initializer

# init(volumeID:volumeName:)

Creates a volume with the given identifier and name.

macOS 15.4+

``` source
init(
    volumeID: FSVolume.Identifier,
    volumeName: FSFileName
)
```

## Parameters 

`volumeID`  

An FSVolume.Identifier to uniquely identify the volume. For a network file system that supports multiple authenticated users, disambiguate the users by using qualifying data in the identifier.

`volumeName`  

A name for the volume.

## See Also

### Creating a volume

class Identifier

A type that identifies a volume.

class FSFileName

The name of a file, expressed as a data buffer.


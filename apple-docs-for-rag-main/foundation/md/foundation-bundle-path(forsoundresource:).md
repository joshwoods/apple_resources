

- Foundation
- Bundle
-  path(forSoundResource:) 

Instance Method

# path(forSoundResource:)

Returns the location of the specified sound resource file.

macOS 10.0+

``` source
func path(forSoundResource name: NSSound.Name) -> String?
```

## Parameters 

`name`  

The name of the sound resource file, without any pathname information. Including a filename extension is optional

## Return Value

The absolute pathname of the resource file or `nil` if the file was not found.

## Discussion

Sound resources are those files in the bundle that are recognized by the `NSSound` class. The types of sound files can be determined by calling the `soundUnfilteredFileTypes` method of `NSSound`.

## See Also

### Related Documentation

func path(forResource: String?, ofType: String?) -> String?

Returns the full pathname for the resource identified by the specified name and file extension.


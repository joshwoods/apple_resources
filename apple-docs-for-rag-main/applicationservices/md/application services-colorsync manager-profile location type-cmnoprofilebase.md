

- Application Services
- ColorSync Manager
- Profile Location Type
-  cmNoProfileBase 

Global Variable

# cmNoProfileBase

The profile is temporary. It will not persist in memory after its use for a color session. You can specify this type of profile location with the `CMNewProfile` and the `CMCopyProfile` functions.

macOS 10.0+

``` source
var cmNoProfileBase: Int { get }
```


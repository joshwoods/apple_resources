

- SceneKit
-  SCNDetailedErrorsKey 

Global Variable

# SCNDetailedErrorsKey

Detailed error information from SceneKit’s scene file loading process.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let SCNDetailedErrorsKey: String
```

## Discussion

If SceneKit reports an error when creating or loading from a scene source, the userInfo dictionary of the returned NSError object may contain this key, whose value is an array of dictionaries (each containing one or more of the keys listed in Scene File Consistency Error Keys) providing details about the location of the error in the scene file.

If you specify true for the checkConsistency option when creating or loading from a scene source, SceneKit verifies the scene file against the specification for its file format. Verifying a scene file can result in additional error reports for violations of the file format specification that do not prevent SceneKit from loading the file.


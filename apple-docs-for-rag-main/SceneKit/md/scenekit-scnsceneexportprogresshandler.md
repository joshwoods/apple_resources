

- SceneKit
-  SCNSceneExportProgressHandler 

Type Alias

# SCNSceneExportProgressHandler

The signature for the block that SceneKit calls during scene export.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias SCNSceneExportProgressHandler = (Float, (any Error)?, UnsafeMutablePointer) -> Void
```

## Discussion

You specify a block with this signature when calling the write(to:options:delegate:progressHandler:) method in order to receive updates on the progress of the export operation. The block takes the following parameters:

totalProgress  
A number between `0.0` and `1.0` that indicates the progress of the export operation, with `0.0` indicating that the operation has just begun and `1.0` indicating the operation has completed.

error  
An error encountered during the export process, or `nil` if no errors have occurred.

stop  
Set `*stop` to true inside the block to cancel export.

## See Also

### Constants

Scene Attributes

Attribute keys available in the options dictionary for the methods attribute(forKey:) and setAttribute(_:forKey:)

Scene Export Options

Options for the write(to:options:delegate:progressHandler:) method.


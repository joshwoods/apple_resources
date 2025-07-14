

- Video Toolbox
-  kVTMultiPassStorageCreationOption_DoNotDelete 

Global Variable

# kVTMultiPassStorageCreationOption_DoNotDelete

Indicates that the multipass storage object’s backing store should not be deleted when finalized.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+

``` source
let kVTMultiPassStorageCreationOption_DoNotDelete: CFString
```

## Discussion

If the backing store file did not exist when the storage was created, the file will be deleted when the multipass storage object is finalized, unless you set this option to kCFBooleanTrue in the options dictionary.


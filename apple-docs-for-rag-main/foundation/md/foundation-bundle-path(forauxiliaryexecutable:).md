

- Foundation
- Bundle
-  path(forAuxiliaryExecutable:) 

Instance Method

# path(forAuxiliaryExecutable:)

Returns the full pathname of the executable with the specified name in the receiver’s bundle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func path(forAuxiliaryExecutable executableName: String) -> String?
```

## Parameters 

`executableName`  

The name of an executable file.

## Return Value

The full pathname of the executable `executableName` in the receiver’s bundle.

## Discussion

This method returns the appropriate path for modern application and framework bundles. This method may not return a path for non-standard bundle formats or for some older bundle formats.

## See Also

### Getting the Standard Bundle Directories

var resourceURL: URL?

The file URL of the bundle’s subdirectory containing resource files.

var executableURL: URL?

The file URL of the receiver’s executable file.

var privateFrameworksURL: URL?

The file URL of the bundle’s subdirectory containing private frameworks.

var sharedFrameworksURL: URL?

The file URL of the receiver’s subdirectory containing shared frameworks.

var builtInPlugInsURL: URL?

The file URL of the receiver’s subdirectory containing plug-ins.

func url(forAuxiliaryExecutable: String) -> URL?

Returns the file URL of the executable with the specified name in the receiver’s bundle.

var sharedSupportURL: URL?

The file URL of the bundle’s subdirectory containing shared support files.

var appStoreReceiptURL: URL?

The file URL for the bundle’s App Store receipt.

Deprecated

var resourcePath: String?

The full pathname of the bundle’s subdirectory containing resources.

var executablePath: String?

The full pathname of the receiver’s executable file.

var privateFrameworksPath: String?

The full pathname of the bundle’s subdirectory containing private frameworks.

var sharedFrameworksPath: String?

The full pathname of the bundle’s subdirectory containing shared frameworks.

var builtInPlugInsPath: String?

The full pathname of the receiver’s subdirectory containing plug-ins.

var sharedSupportPath: String?

The full pathname of the bundle’s subdirectory containing shared support files.


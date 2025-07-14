

- Foundation
- Bundle
-  sharedSupportURL 

Instance Property

# sharedSupportURL

The file URL of the bundle’s subdirectory containing shared support files.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var sharedSupportURL: URL? { get }
```

## Discussion

This property contains the appropriate path for modern application and framework bundles. This property may not contain a path for non-standard bundle formats or for some older bundle formats.

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

func path(forAuxiliaryExecutable: String) -> String?

Returns the full pathname of the executable with the specified name in the receiver’s bundle.

var sharedSupportPath: String?

The full pathname of the bundle’s subdirectory containing shared support files.


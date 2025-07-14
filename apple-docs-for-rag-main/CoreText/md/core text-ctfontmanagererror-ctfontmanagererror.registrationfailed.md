

- Core Text
- CTFontManagerError
-  CTFontManagerError.registrationFailed 

Case

# CTFontManagerError.registrationFailed

An error that indicates the file can’t be processed due to an unexpected FontProvider error.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case registrationFailed
```

## See Also

### Constants

case fileNotFound

An error that indicates the file doesn’t exist at the specified URL.

case insufficientPermissions

An error that indicates insufficient permissions to access the file.

case unrecognizedFormat

An error that indicates the file’s format is unrecognized or unsupported.

case invalidFontData

An error that indicates the file contains invalid font data that could cause system problems.

case alreadyRegistered

An error that indicates the file is already registered in the specified scope.

case exceededResourceLimit

An error that indicates an operation failure due to a system limitation.

case assetNotFound

An error that indicates the asset isn’t found.

case notRegistered

An error that indicates the file isn’t registered in the specified scope.

case inUse

An error that indicates the font file is actively in use and can’t be unregistered.

case systemRequired

An error that indicates the file is required by the system and can’t be unregistered.

case missingEntitlement

An error that indicates the file can’t be processed because the provider doesn’t have a necessary entitlement.

case insufficientInfo

An error that indicates the font descriptor doesn’t have the necessary information to specify a font file.

case cancelledByUser

An error that indicates the user cancelled the operation.

case duplicatedName

An error that indicates the file can’t register because of a duplicate font name.

case invalidFilePath

An error that indicates the file isn’t in an allowed location, which must be either in the app’s bundle or an on-demand resource.


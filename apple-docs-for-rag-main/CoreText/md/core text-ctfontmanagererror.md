

- Core Text
-  CTFontManagerError 

Enumeration

# CTFontManagerError

Errors that prevent unregistration of fonts for a specified font file URL.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTFontManagerError
```

## Topics

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

case registrationFailed

An error that indicates the file can’t be processed due to an unexpected FontProvider error.

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

case unsupportedScope

An error that indicates the specified scope isn’t supported.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum CTFontDescriptorMatchingState

Constants that track the progress of font descriptor matching.

enum CTFontManagerAutoActivationSetting

Sets the auto-activation for the specified bundle identifier.

enum CTFontManagerScope

Constants that define the scope for font registration.

struct CTLineBoundsOptions

Options for getting the bounds of a line of text.

enum CTRubyAlignment

Constants that specify how to align the ruby text and the base text relative to each other when they have different lengths.

enum CTRubyOverhang

Constants that specify whether, and on which side, ruby text can overhang adjacent text if it’s wider than the base text.

enum CTRubyPosition

Constants that specify the position of the ruby text relative to to the base text.


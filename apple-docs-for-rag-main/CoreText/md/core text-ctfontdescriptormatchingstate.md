

- Core Text
-  CTFontDescriptorMatchingState 

Enumeration

# CTFontDescriptorMatchingState

Constants that track the progress of font descriptor matching.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTFontDescriptorMatchingState
```

## Topics

### Constants

case didBegin

A state that indicates matching is about to begin.

case didFinish

A state that indicates matching is done.

case willBeginQuerying

A state that indicates communication with the server is about to begin.

case stalled

A state that indicates that matching is stalled, such as while waiting for a server response.

case willBeginDownloading

A state that indicates downloading is about to begin.

case downloading

A state that indicates downloading is in progress.

case didFinishDownloading

A state that indicates downloading is done.

case didMatch

A state that indicates the font descriptor match is successful.

case didFailWithError

A state that indicates an error.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

enum CTFontManagerAutoActivationSetting

Sets the auto-activation for the specified bundle identifier.

enum CTFontManagerError

Errors that prevent unregistration of fonts for a specified font file URL.

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


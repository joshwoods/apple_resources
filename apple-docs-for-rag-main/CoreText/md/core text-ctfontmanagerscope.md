

- Core Text
-  CTFontManagerScope 

Enumeration

# CTFontManagerScope

Constants that define the scope for font registration.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CTFontManagerScope
```

## Overview

On macOS, a user session refers to a login session. On iOS, a user session refers to the current booted session.

## Topics

### Constants

case none

No scope is defined.

case process

The font is available to the current process for the duration of the process unless directly unregistered.

case persistent

The font is available to all processes for the current user session and will be available in subsequent sessions unless unregistered.

case session

The font is available to the current user session but won’t be available in subsequent sessions.

static var user: CTFontManagerScope

The font is available to all processes for the current user session and will be available in subsequent sessions unless unregistered.

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

enum CTFontDescriptorMatchingState

Constants that track the progress of font descriptor matching.

enum CTFontManagerAutoActivationSetting

Sets the auto-activation for the specified bundle identifier.

enum CTFontManagerError

Errors that prevent unregistration of fonts for a specified font file URL.

struct CTLineBoundsOptions

Options for getting the bounds of a line of text.

enum CTRubyAlignment

Constants that specify how to align the ruby text and the base text relative to each other when they have different lengths.

enum CTRubyOverhang

Constants that specify whether, and on which side, ruby text can overhang adjacent text if it’s wider than the base text.

enum CTRubyPosition

Constants that specify the position of the ruby text relative to to the base text.


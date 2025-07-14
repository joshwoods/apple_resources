

- Media Player
-  MPLanguageOptionCharacteristicIsMainProgramContent 

Global Variable

# MPLanguageOptionCharacteristicIsMainProgramContent

Indicates that the language option includes content that’s marked by the content author as intrinsic to the presentation of the language option.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
let MPLanguageOptionCharacteristicIsMainProgramContent: String
```

## Discussion

An option that presents the main program audio for the presentation, regardless of locale, would typically have this characteristic. The system infers the presence of this characteristic for a language option and considers any option that doesn’t have the characteristic MPLanguageOptionCharacteristicIsAuxiliaryContent to have the characteristic.

## See Also

### Language option characteristic constants

let MPLanguageOptionCharacteristicContainsOnlyForcedSubtitles: String

Indicates that the language option presents only forced subtitles.

let MPLanguageOptionCharacteristicDescribesMusicAndSound: String

Indicates that the language option includes legible content in the language of its specified locale that describes music and sound effects occurring in program audio.

let MPLanguageOptionCharacteristicDescribesVideo: String

Indicates that the language option includes audible content that describes the visual portion of the presentation.

let MPLanguageOptionCharacteristicDubbedTranslation: String

Indicates that the language option includes content that contains a dubbed translation.

let MPLanguageOptionCharacteristicEasyToRead: String

Indicates that the language option provides legible content in the language of its specified locale and that the content was edited for ease of reading.

let MPLanguageOptionCharacteristicIsAuxiliaryContent: String

Indicates that the language option includes content that’s marked by the content author as auxiliary to the presentation of the language option.

let MPLanguageOptionCharacteristicLanguageTranslation: String

Indicates that the language option contains a translation in the language of its specified locale.

let MPLanguageOptionCharacteristicTranscribesSpokenDialog: String

Indicates that the language option includes legible content in the language of its specified locale that transcribes spoken dialog.

let MPLanguageOptionCharacteristicVoiceOverTranslation: String

Indicates that the language option includes voice over content in the language of its specified locale describes translated dialog.


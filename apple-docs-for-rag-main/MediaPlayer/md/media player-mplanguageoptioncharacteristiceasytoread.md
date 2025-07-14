

- Media Player
-  MPLanguageOptionCharacteristicEasyToRead 

Global Variable

# MPLanguageOptionCharacteristicEasyToRead

Indicates that the language option provides legible content in the language of its specified locale and that the content was edited for ease of reading.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
let MPLanguageOptionCharacteristicEasyToRead: String
```

## Discussion

Closed caption tracks that carry easy reader captions (per the CEA-608 specification) should have this characteristic tag. Subtitle tracks can also have this characteristic tag, where appropriate.

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

let MPLanguageOptionCharacteristicIsAuxiliaryContent: String

Indicates that the language option includes content that’s marked by the content author as auxiliary to the presentation of the language option.

let MPLanguageOptionCharacteristicIsMainProgramContent: String

Indicates that the language option includes content that’s marked by the content author as intrinsic to the presentation of the language option.

let MPLanguageOptionCharacteristicLanguageTranslation: String

Indicates that the language option contains a translation in the language of its specified locale.

let MPLanguageOptionCharacteristicTranscribesSpokenDialog: String

Indicates that the language option includes legible content in the language of its specified locale that transcribes spoken dialog.

let MPLanguageOptionCharacteristicVoiceOverTranslation: String

Indicates that the language option includes voice over content in the language of its specified locale describes translated dialog.


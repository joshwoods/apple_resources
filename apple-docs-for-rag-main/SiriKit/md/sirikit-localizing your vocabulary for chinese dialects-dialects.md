

- SiriKit
-  Localizing Your Vocabulary for Chinese Dialects 

Article

# Localizing Your Vocabulary for Chinese Dialects

Apply emphasis markers to your pronunciation tips to assist Siri with Chinese dialects.

## Overview

For specific localizations, additional rules apply when specify values for the `VocabularyItemPronunciation` key:

- zh_CN: China Mandarin localization:

- Tones are represented using the numbers 1, 2, 3, 4, and 5. Use the number 5 for the neutral tone. Place tones at the end of the Pinyin representation of each character. For example, `ping2 guo3`.

- You can replace the special character `ü` in Pinyin with `yu`. For example, `nü` would become `nyu`.

- zh_TW: Taiwan Mandarin localization:

- Tones are represented using the numbers 1, 2, 3, 4, and 5. Use the number 5 for the neutral tone. Place tones at the end of the Pinyin representation of each character. For example, 蘇打綠 becomes `su1 da3 lyu4`.

- zh_HK: Hong Kong Cantonese localization:

- Use the Jyutping 粤语拼音 (粤拼) romanization system for Cantonese.

- Tones are represented using the numbers 1, 2, 3, 4, 5, and 6. Place tone numbers at the end of the Jyutping. For example, 的士 becomes `dik1 si2`, and 短訊 becomes `dyun2 seon2`.

## See Also

### Articles

Adding User Interactivity with Siri Shortcuts and the Shortcuts App

Add custom intents and parameters to help users interact more quickly and effectively with Siri and the Shortcuts app.

Defining Relevant Shortcuts for the Siri Watch Face

Inform Siri when your app’s shortcuts may be useful to the user.

Deleting Donated Shortcuts

Remove your donations from Siri.

Dispatching intents to handlers

Provide SiriKit with an intent handler capable of handling a specific intent.

Improving Siri Media Interactions and App Selection

Fine-tune voice controls and improve Siri Suggestions by sharing app capabilities, customized names, and listening habits with the system.

Improving interactions between Siri and your messaging app

Donate app-specific content, use Siri’s contact suggestions, and adopt the latest platform features to create a more consistent messaging experience.

Registering Custom Vocabulary with SiriKit

Register your app’s custom terminology, and provide sample phrases for how to use your app with Siri.

Confirming the Details of an Intent

Perform final validation of the intent parameters and verify that your services are ready to fulfill the intent.

Handling an Intent

Fulfill the intent and provide feedback to SiriKit about what you did.

Resolving the Parameters of an Intent

Validate the parameters of an intent and make sure that you have the information you need to continue.

Generating a List of Ride Options

Generate ride options for Maps to display to the user.

Handling the Ride-Booking Intents

Support the different intent-handling sequences for booking rides with Shortcuts or Maps.

Displaying Shortcut Information in a Siri Watch Face Card

Display and customize watch-specific shortcut information with a default card template.

Donating Reservations

Inform Siri of reservations made from your app.

Defining Relevant Shortcuts for the Siri Watch Face

Inform Siri when your app’s shortcuts may be useful to the user.


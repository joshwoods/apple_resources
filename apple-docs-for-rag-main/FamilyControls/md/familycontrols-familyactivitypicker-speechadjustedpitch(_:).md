

- FamilyControls
- FamilyActivityPicker
-  speechAdjustedPitch(\_:) 

Instance Method

# speechAdjustedPitch(\_:)

Raises or lowers the pitch of spoken text.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func speechAdjustedPitch(_ value: Double) -> some View
```

## Parameters 

`value`  

The amount to raise or lower the pitch. Values between `-1` and `0` result in a lower pitch while values between `0` and `1` result in a higher pitch. The method clamps values to the range `-1` to `1`.

## Discussion

Use this modifier when you want to change the pitch of spoken text. The value indicates how much higher or lower to change the pitch.

## See Also

### VoiceOver

func speechAlwaysIncludesPunctuation(Bool) -> some View

Sets whether VoiceOver should always speak all punctuation in the text view.

func speechAnnouncementsQueued(Bool) -> some View

Controls whether to queue pending announcements behind existing speech rather than interrupting speech in progress.

func speechSpellsOutCharacters(Bool) -> some View

Sets whether VoiceOver should speak the contents of the text view character by character.


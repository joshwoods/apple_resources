

- Foundation
- NSLinguisticTagger
-  stringEdited(in:changeInLength:) Deprecated

Instance Method

# stringEdited(in:changeInLength:)

Notifies the linguistic tagger that the string (if mutable) has changed as specified by the parameters.

iOS 5.0–18.4DeprecatediPadOS 5.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.7–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
func stringEdited(
    in newRange: NSRange,
    changeInLength delta: Int
)
```

Deprecated

All NSLinguisticTagger API should be replaced with NaturalLanguage.framework API

## Parameters 

`newRange`  

The range in the final string that was edited.

`delta`  

The change in length.


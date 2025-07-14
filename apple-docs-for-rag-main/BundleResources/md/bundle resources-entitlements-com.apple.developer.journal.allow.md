

- Bundle Resources
- Entitlements
-  com.apple.developer.journal.allow 

Property List Key

# com.apple.developer.journal.allow

The entitlement that enables an app to present the journaling suggestions picker.

iOS 17.2+iPadOS 17.2+

## Details 

Type  

array of strings

## Possible Values 

`suggestions`  

## Discussion

The Journaling Suggestions framework can’t present the JournalingSuggestionsPicker for apps without this entitlement in their code signature. Add this entitlement to your app by enabling the Journaling Suggestions capability in Xcode.

For more information about presenting journaling suggestions in your app, see Presenting the suggestions picker and processing a selection.


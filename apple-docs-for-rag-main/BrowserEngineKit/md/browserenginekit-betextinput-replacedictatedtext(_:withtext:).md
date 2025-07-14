

- BrowserEngineKit
- BETextInput
-  replaceDictatedText(\_:withText:) 

Instance Method

# replaceDictatedText(\_:withText:)

Inserts/replaces text for a dictation.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func replaceDictatedText(
    _ oldText: String,
    withText newText: String
)
```

**Required**

## See Also

### Dictation

func willInsertFinalDictationResult()

Indicates the system is about to insert the final dictation result.

**Required**

func didInsertFinalDictationResult()

Indicates system has inserted the final dictation result

**Required**


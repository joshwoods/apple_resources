

- Translation
- TranslationSession
-  translate(\_:) 

Instance Method

# translate(\_:)

Translates a single string of text.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
func translate(_ string: String) async throws -> TranslationSession.Response
```

## Parameters 

`string`  

The string of text to translate.

## Return Value

The response containing the text translation.

## Discussion

This function translates a single line of text and might display different UI depending on the state of the translation. The languages the framework requires for the translation don’t have to be installed before calling this method.

If the required languages for translation have already downloaded and the source language is clear, this function returns results without showing any UI to the user.

If the source or target language aren’t installed, the framework asks the user for permission to download the languages. During download a progress indicator displays. After the download completes, the framework performs the translation.

If the `sourceLanguage` is `nil` and the framework can’t detect the source language from the content, the framework prompts the user to choose the source language.

This function throws an `Error` if:

- the user doesn’t agree to downloading the languages

- the user dismisses the progress UI while the languages download,

- the TranslationSession fails to validate, or

- something goes wrong while performing the translation.

If someone dismisses the progress UI while the languages download, the system throws a `CocoaError/userCancelled` error, and the languages continue to download in the background.

Note

Calls to this function can take several minutes while languages download.

## See Also

### Translating text

func translate(batch: [TranslationSession.Request]) -> TranslationSession.BatchResponse

Translates multiple strings of text of the same language, returning a sequence of responses as they’re available.

func translations(from: [TranslationSession.Request]) async throws -> [TranslationSession.Response]

Translates multiple strings of text of the same language, returning the results all at once when complete.

struct Request

A translation request containing a single item of text to translate.

struct Response

The response to a translation request.

struct BatchResponse

A type that provides asynchronous access to translation responses.


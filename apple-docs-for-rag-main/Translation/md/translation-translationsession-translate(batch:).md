

- Translation
- TranslationSession
-  translate(batch:) 

Instance Method

# translate(batch:)

Translates multiple strings of text of the same language, returning a sequence of responses as they’re available.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
func translate(batch: [TranslationSession.Request]) -> TranslationSession.BatchResponse
```

## Parameters 

`batch`  

The array of requests to translate.

## Return Value

An `AsyncSequence` of responses containing the text translations.

## Discussion

This function translates multiple strings of text incrementally and might display different UI depending on the state of the translation. The languages the framework requires for the translation don’t have to be installed before calling this method.

Pass in the strings of text you want to translate as an array of type TranslationSession.Request. Set the clientIdentifier on each request so you can match the request with the response as the translations incrementally return.

If the required languages for translation have already downloaded and the source language is clear, this function returns results without showing any UI to the user.

If the source or target language aren’t installed, the framework asks the user for permission to download the languages. During download a progress indicator displays. After the download completes, the framework performs the translation.

If the `sourceLanguage` is `nil` and the framework can’t detect the source language from the content, the framework prompts the user to choose the source language.

The framework only supports string translations of the same language. The strings must either match the `sourceLanguage` you set in the configuration, or if the `sourceLanguage` is `nil`, be of the same language.

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

func translate(String) async throws -> TranslationSession.Response

Translates a single string of text.

func translations(from: [TranslationSession.Request]) async throws -> [TranslationSession.Response]

Translates multiple strings of text of the same language, returning the results all at once when complete.

struct Request

A translation request containing a single item of text to translate.

struct Response

The response to a translation request.

struct BatchResponse

A type that provides asynchronous access to translation responses.


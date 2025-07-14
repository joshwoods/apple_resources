

- Translation
- TranslationSession
-  TranslationSession.Response 

Structure

# TranslationSession.Response

The response to a translation request.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
struct Response
```

## Overview

You get a single response structure after you translate a string, or when you call one of the batch translation methods passing in an array of translation requests. When the translation completes, a response instance returns with the translation result along with properties the framework used to perform the translation.

## Topics

### Initializers

init(sourceLanguage: Locale.Language, targetLanguage: Locale.Language, sourceText: String, targetText: String, clientIdentifier: String?)

Creates an instance of a translation response.

### Instance Properties

let clientIdentifier: String?

The unique identifier matching the client identifier set in the translation request.

let sourceLanguage: Locale.Language

The language that the framework translated the text from.

let sourceText: String

The original text to translate from.

let targetLanguage: Locale.Language

The language that the framework translated the text into.

let targetText: String

The result of the translation.

## Relationships

### Conforms To

- Sendable

## See Also

### Translating text

func translate(String) async throws -> TranslationSession.Response

Translates a single string of text.

func translate(batch: [TranslationSession.Request]) -> TranslationSession.BatchResponse

Translates multiple strings of text of the same language, returning a sequence of responses as they’re available.

func translations(from: [TranslationSession.Request]) async throws -> [TranslationSession.Response]

Translates multiple strings of text of the same language, returning the results all at once when complete.

struct Request

A translation request containing a single item of text to translate.

struct BatchResponse

A type that provides asynchronous access to translation responses.


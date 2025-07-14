

- Translation
- TranslationSession
-  TranslationSession.Request 

Structure

# TranslationSession.Request

A translation request containing a single item of text to translate.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
struct Request
```

## Overview

Create a translation request to translate a string of text. Create the request using the init(sourceText:clientIdentifier:) initializer. Set the `sourceText` to the string of text you want to translate. Then pass that request in an array to one of the batch translation functions.

Keep track of which responses correspond with which requests by setting the clientIdentifier on the request you send, then matching it against the clientIdentifier response you receive when the translation completes and returns.

## Topics

### Initializers

init(sourceText: String, clientIdentifier: String?)

Creates a request for translating a single string of text.

### Instance Properties

var clientIdentifier: String?

An optional unique identifier to associate a translation request with its response.

var sourceText: String

The input text the framework translates.

## See Also

### Translating text

func translate(String) async throws -> TranslationSession.Response

Translates a single string of text.

func translate(batch: [TranslationSession.Request]) -> TranslationSession.BatchResponse

Translates multiple strings of text of the same language, returning a sequence of responses as they’re available.

func translations(from: [TranslationSession.Request]) async throws -> [TranslationSession.Response]

Translates multiple strings of text of the same language, returning the results all at once when complete.

struct Response

The response to a translation request.

struct BatchResponse

A type that provides asynchronous access to translation responses.


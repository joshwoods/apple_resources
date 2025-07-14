

- Translation
- TranslationSession
-  TranslationSession.BatchResponse 

Structure

# TranslationSession.BatchResponse

A type that provides asynchronous access to translation responses.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
struct BatchResponse
```

## Overview

This type returns instances of TranslationSession.Response asynchronously and throws an `Error` if something goes wrong.

## Topics

### Structures

struct AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

### Instance Methods

func makeAsyncIterator() -> TranslationSession.BatchResponse.AsyncIterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

### Type Aliases

typealias Element

The type of element produced by this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

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

struct Response

The response to a translation request.


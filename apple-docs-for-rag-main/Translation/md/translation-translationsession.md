

- Translation
-  TranslationSession 

Class

# TranslationSession

A class that performs translations between a pair of languages.

iOS 18.0+iPadOS 18.0+macOS 15.0+

``` source
class TranslationSession
```

## Overview

You don’t instantiate this class directly. Instead, you obtain an instance of it by adding a translationTask(_:action:) or translationTask(source:target:action:) function to the SwiftUI view containing the content you want to translate, such as a Text view. When you do, the function passes you an instance of a translation session in its `action` closure which triggers as soon as the view appears. After you receive this instance, use one of the translate functions to translate one or more strings of text.

The following example demonstrates how to translate a single string of text:

```
struct TranslationExample: View {
    var sourceText: String
    var sourceLanguage: Locale.Language?
    var targetLanguage: Locale.Language?

    @State private var targetText: String?

    var body: some View {
        Text(targetText ?? sourceText)
            .translationTask(
                source: sourceLanguage,
                target: targetLanguage
            ) { session in
                do {
                    let response = try await session.translate(sourceText)
                    targetText = response.targetText
                } catch {
                    // Handle error.
                }
            }
    }
}
```

Note

All translations using the `TranslationSession` class are processed on the user’s device. Apple may collect API usage and performance metrics including the app bundle ID and the original and translated language, but this data does not include the original or translated content.

## Topics

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

struct BatchResponse

A type that provides asynchronous access to translation responses.

### Preparing for translation

struct Configuration

A type containing the information to use when performing a translation.

func prepareTranslation() async throws

Asks the user for permission to download translation languages without doing any translations.

### Getting configuration

let sourceLanguage: Locale.Language?

The input language to translate from.

let targetLanguage: Locale.Language?

The output language to translate into.

## See Also

### Essentials

Translating text within your app

Display simple system translations and create custom translation experiences.

nonisolated func translationPresentation(isPresented: Binding&lt;Bool>, text: String, attachmentAnchor: PopoverAttachmentAnchor = .rect(.bounds), arrowEdge: Edge = .top, replacementAction: ((String) -> Void)? = nil) -> some View 

Presents a translation popover when a given condition is true.

nonisolated func translationTask(_ configuration: TranslationSession.Configuration?, action: @escaping (TranslationSession) async -> Void) -> some View 

Adds a task to perform before this view appears or when the translation configuration changes.

nonisolated func translationTask(source: Locale.Language? = nil, target: Locale.Language? = nil, action: @escaping (TranslationSession) async -> Void) -> some View 

Adds a task to perform before this view appears or when the specified source or target languages change.


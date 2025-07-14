

- App Intents
-  IntentItemCollection 

Structure

# IntentItemCollection

Return this object to provide an advanced list of options, optionally divided in sections.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentItemCollection where Result : _IntentValue
```

## Example

```
struct CreateBookIntent: AppIntent {
    @Parameter(title: "Author Name", optionsProvider: AuthorNamesOptionsProvider())
    var authorName: String

    struct AuthorNamesOptionsProvider: DynamicOptionsProvider {
        func results() async throws -> ItemCollection {
            ItemCollection {
                ItemSection("Italian Authors") {
                    "Dante Alighieri"
                    "Alessandro Manzoni"
                }
                ItemSection("Russian Authors") {
                    "Anton Chekhov"
                    "Fyodor Dostoevsky"
                }
            }
        }
    }
}
```

## Topics

### Initializers

init(promptLabel: LocalizedStringResource?, usesIndexedCollation: Bool, items: [Result])

Create a `ItemCollection` containing `Items`, or one or more `Sections`.

init(promptLabel: LocalizedStringResource?, usesIndexedCollation: Bool, sections: [IntentItemSection&lt;Result>])

Create an `ItemCollection` containing one or more `Sections`.

init(promptLabel: LocalizedStringResource?, usesIndexedCollation: Bool, sectionsBuilder: () -> [IntentItemSection&lt;Result>])

Create an `ItemCollection` containing `Items`, or one or more `Sections` provided by a builder.

### Instance Properties

var items: [Result.ValueType]

Returns all results as an array.

var promptLabel: LocalizedStringResource?

A text prompt shown at the top of the view that presents the options.

var sections: [IntentItemSection&lt;Result>]

var usesIndexedCollation: Bool

If set to true, presents the list of options with an alphabetical index on the right side of the screen (table view section index titles).

### Type Properties

static var empty: IntentItemCollection&lt;Result>

Returns an empty result.

## Relationships

### Conforms To

- ResultsCollection

## See Also

### Items and collections

struct IntentItem

A type describing a value returned from a dynamic options provider, plus information about how to display it to users.

struct IntentItemSection

An object you use to divide dynamic options into sections.

struct IntentCollectionSize


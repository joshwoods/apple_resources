

- SwiftUI
- View
-  searchable(text:tokens:placement:prompt:token:) 

Instance Method

# searchable(text:tokens:placement:prompt:token:)

Marks this view as searchable with text and tokens.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
nonisolated
func searchable(
    text: Binding,
    tokens: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: S,
    @ViewBuilder token: @escaping (C.Element) -> T
) -> some View where C : RandomAccessCollection, C : RangeReplaceableCollection, T : View, S : StringProtocol, C.Element : Identifiable
```

Show all declarations

## Parameters 

`text`  

The text to display and edit in the search field.

`tokens`  

A collection of tokens to display and edit in the search field.

`placement`  

The preferred placement of the search field within the containing view hierarchy.

`prompt`  

A string representing the prompt of the search field which provides users with guidance on what to search for.

`token`  

A view builder that creates a view given an element in tokens.

## Mentioned in 

Performing a search operation

## Discussion

For more information about using searchable modifiers, see Adding a search interface to your app.

## See Also

### Searching your app’s data model

Adding a search interface to your app

Present an interface that people can use to search for content in your app.

Performing a search operation

Update search results based on search text and optional tokens that you store.

func searchable(text:placement:prompt:)

Marks this view as searchable, which configures the display of a search field.

func searchable(text:editableTokens:placement:prompt:token:)

Marks this view as searchable, which configures the display of a search field.

struct SearchFieldPlacement

The placement of a search field in a view hierarchy.


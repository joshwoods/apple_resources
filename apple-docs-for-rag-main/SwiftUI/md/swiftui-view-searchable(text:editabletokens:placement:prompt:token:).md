

- SwiftUI
- View
-  searchable(text:editableTokens:placement:prompt:token:) 

Instance Method

# searchable(text:editableTokens:placement:prompt:token:)

Marks this view as searchable, which configures the display of a search field.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func searchable(
    text: Binding,
    editableTokens: Binding,
    placement: SearchFieldPlacement = .automatic,
    prompt: LocalizedStringKey,
    @ViewBuilder token: @escaping (Binding) -> some View
) -> some View where C : RandomAccessCollection, C : RangeReplaceableCollection, C.Element : Identifiable
```

Show all declarations

## Parameters 

`text`  

The text to display and edit in the search field.

`editableTokens`  

A collection of tokens to display and edit in the search field.

`placement`  

The preferred placement of the search field within the containing view hierarchy.

`prompt`  

The key for the localized prompt of the search field which provides users with guidance on what to search for.

`token`  

A view builder that creates a view given an element in tokens.

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

func searchable(text:tokens:placement:prompt:token:)

Marks this view as searchable with text and tokens.

struct SearchFieldPlacement

The placement of a search field in a view hierarchy.


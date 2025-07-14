

- SwiftUI
- View fundamentals
- View
-  Search modifiers 

API Collection

# Search modifiers

Enable people to search for content in your app.

## Overview

Use search view modifiers to add search capability to your app. For more information, see Search.

## Topics

### Displaying a search interface

func searchable(text:placement:prompt:)

Marks this view as searchable, which configures the display of a search field.

func searchable(text:isPresented:placement:prompt:)

Marks this view as searchable with programmatic presentation of the search field.

func searchPresentationToolbarBehavior(SearchPresentationToolbarBehavior) -> some View

Configures the search toolbar presentation behavior for any searchable modifiers within this view.

### Searching with tokens

func searchable(text:tokens:placement:prompt:token:)

Marks this view as searchable with text and tokens.

func searchable(text:tokens:isPresented:placement:prompt:token:)

Marks this view as searchable with text and tokens, as well as programmatic presentation.

### Searching with editable tokens

func searchable(text:editableTokens:isPresented:placement:prompt:token:)

Marks this view as searchable, which configures the display of a search field.

func searchable(text:editableTokens:placement:prompt:token:)

Marks this view as searchable, which configures the display of a search field.

### Making search suggestions

func searchSuggestions&lt;S>(() -> S) -> some View

Configures the search suggestions for this view.

func searchSuggestions(Visibility, for: SearchSuggestionsPlacement.Set) -> some View

Configures how to display search suggestions within this view.

func searchCompletion(_:)

Associates a fully formed string with the value of this view when used as a search suggestion.

func searchable(text:tokens:suggestedTokens:placement:prompt:token:)

Marks this view as searchable with text, tokens, and suggestions.

func searchable(text:tokens:suggestedTokens:isPresented:placement:prompt:token:)

Marks this view as searchable with text, tokens, and suggestions, as well as programmatic presentation.

### Limiting search scope

func searchScopes&lt;V, S>(Binding&lt;V>, scopes: () -> S) -> some View

Configures the search scopes for this view.

func searchScopes&lt;V, S>(Binding&lt;V>, activation: SearchScopeActivation, () -> S) -> some View

Configures the search scopes for this view with the specified activation strategy.

### Searching through dictation

func searchDictationBehavior(TextInputDictationBehavior) -> some View

Configures the dictation behavior for any search fields configured by the searchable modifier.

## See Also

### Providing interactivity

Input and event modifiers

Supply actions for a view to perform in response to user input and system events.

Presentation modifiers

Define additional views for the view to present under specified conditions.

State modifiers

Access storage and provide child views with configuration data.


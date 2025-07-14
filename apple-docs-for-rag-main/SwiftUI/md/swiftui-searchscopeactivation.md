

- SwiftUI
-  SearchScopeActivation 

Structure

# SearchScopeActivation

The ways that searchable modifiers can show or hide search scopes.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
struct SearchScopeActivation
```

## Mentioned in 

Scoping a search operation

## Topics

### Getting search scope activiation types

static var automatic: SearchScopeActivation

The automatic activation of the scope bar.

static var onSearchPresentation: SearchScopeActivation

An activation where the system shows search scopes after presenting search and hides search scopes after search cancellation.

static var onTextEntry: SearchScopeActivation

An activation where the system shows search scopes when typing begins in the search field and hides search scopes after search cancellation.

## See Also

### Limiting search scope

Scoping a search operation

Divide the search space into a few broad categories.

func searchScopes&lt;V, S>(Binding&lt;V>, scopes: () -> S) -> some View

Configures the search scopes for this view.

func searchScopes&lt;V, S>(Binding&lt;V>, activation: SearchScopeActivation, () -> S) -> some View

Configures the search scopes for this view with the specified activation strategy.




- SwiftUI
- SearchScopeActivation
-  automatic 

Type Property

# automatic

The automatic activation of the scope bar.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
static var automatic: SearchScopeActivation { get }
```

## Discussion

By default, this is onTextEntry in iOS and onSearchPresentation in macOS.

## See Also

### Getting search scope activiation types

static var onSearchPresentation: SearchScopeActivation

An activation where the system shows search scopes after presenting search and hides search scopes after search cancellation.

static var onTextEntry: SearchScopeActivation

An activation where the system shows search scopes when typing begins in the search field and hides search scopes after search cancellation.


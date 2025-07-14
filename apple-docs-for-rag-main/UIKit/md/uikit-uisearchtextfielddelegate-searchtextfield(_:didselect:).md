

- UIKit
- UISearchTextFieldDelegate
-  searchTextField(\_:didSelect:) 

Instance Method

# searchTextField(\_:didSelect:)

Tells the delegate when a person selects a search suggestion in the search text field.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func searchTextField(
    _ searchTextField: UISearchTextField,
    didSelect suggestion: any UISearchSuggestion
)
```

## Parameters 

`searchTextField`  

The search text field displaying search suggestions.

`suggestion`  

The suggestion a person selects.

## Discussion

Implement this method to execute any necessary updates when a person chooses a search suggestion.




- Core Spotlight
- CSUserQuery
-  userEngaged(\_:visibleItems:interaction:) 

Instance Method

# userEngaged(\_:visibleItems:interaction:)

Notifies the system that someone engaged with a specific search result in your app’s interface.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
func userEngaged(
    _ item: CSUserQuery.Item,
    visibleItems: [CSUserQuery.Item],
    interaction: CSUserQuery.UserInteractionKind
)
```

## Parameters 

`item`  

The search result that someone chose.

`visibleItems`  

The set of search results your app was displaying.

## Discussion

When someone selects or interacts with a specific search result in your app’s UI, call this method to tell Spotlight about the interaction. Reporting this type of engagement helps Spotlight deliver better results more quickly in future queries. It also improves the ranked results Spotlight delivers to your app. The system keeps all information about these interactions on the current device

## See Also

### Improving the quality of ranked results

func userEngaged(CSUserQuery.Suggestion, visibleSuggestions: [CSUserQuery.Suggestion], interaction: CSUserQuery.UserInteractionKind)

Notifies the system that someone engaged with a specific text completion in your app’s interface.

enum UserInteractionKind

Constants that indicate how someone engaged with search-related content.


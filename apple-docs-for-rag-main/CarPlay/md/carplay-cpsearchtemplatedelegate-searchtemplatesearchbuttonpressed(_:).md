

- CarPlay
- CPSearchTemplateDelegate
-  searchTemplateSearchButtonPressed(\_:) 

Instance Method

# searchTemplateSearchButtonPressed(\_:)

Tells the delegate that the user tapped the keyboard’s search button.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func searchTemplateSearchButtonPressed(_ searchTemplate: CPSearchTemplate)
```

## Parameters 

`searchTemplate`  

The current search template.

## Discussion

Your implementation of this method should retrieve the search result, and display a CPListTemplate containing the search result items by calling pushTemplate(_:animated:completion:).


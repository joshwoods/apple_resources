

- CarPlay
- CPSearchTemplateDelegate
-  searchTemplate(\_:selectedResult:completionHandler:) 

Instance Method

# searchTemplate(\_:selectedResult:completionHandler:)

Tells the delegate that the user selected an item from the search result.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func searchTemplate(
    _ searchTemplate: CPSearchTemplate,
    selectedResult item: CPListItem,
    completionHandler: @escaping () -> Void
)
```

``` source
func searchTemplate(
    _ searchTemplate: CPSearchTemplate,
    selectedResult item: CPListItem
) async
```

**Required**

## Parameters 

`searchTemplate`  

The current search template.

`item`  

The search result item selected by the user.

`completionHandler`  

The block that you must call after processing the selected result item.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func searchTemplate(_ searchTemplate: CPSearchTemplate, selectedResult item: CPListItem) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Your implementation must call the completion handler after processing the selected result item.


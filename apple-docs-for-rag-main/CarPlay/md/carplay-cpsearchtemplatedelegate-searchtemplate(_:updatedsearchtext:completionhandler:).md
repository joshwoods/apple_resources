

- CarPlay
- CPSearchTemplateDelegate
-  searchTemplate(\_:updatedSearchText:completionHandler:) 

Instance Method

# searchTemplate(\_:updatedSearchText:completionHandler:)

Tells the delegate that the user updated the search criteria text.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func searchTemplate(
    _ searchTemplate: CPSearchTemplate,
    updatedSearchText searchText: String,
    completionHandler: @escaping ([CPListItem]) -> Void
)
```

``` source
func searchTemplate(
    _ searchTemplate: CPSearchTemplate,
    updatedSearchText searchText: String
) async -> [CPListItem]
```

**Required**

## Parameters 

`searchTemplate`  

The current search template.

`searchText`  

The search criteria text entered by the user.

`completionHandler`  

The block your implementation calls after retrieving the search result.

searchResults  
An array of CPListItem objects—one list item for each search result item.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func searchTemplate(_ searchTemplate: CPSearchTemplate, updatedSearchText searchText: String) async -> [CPListItem]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

After the method retrieves the search result, the method must call `completionHandler` for the system to display the result to the user.


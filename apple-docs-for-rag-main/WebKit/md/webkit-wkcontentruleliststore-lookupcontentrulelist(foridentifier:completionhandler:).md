

- WebKit
- WKContentRuleListStore
-  lookUpContentRuleList(forIdentifier:completionHandler:) 

Instance Method

# lookUpContentRuleList(forIdentifier:completionHandler:)

Searches asynchronously for a specific rule list in the data store.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func lookUpContentRuleList(
    forIdentifier identifier: String!,
    completionHandler: ((WKContentRuleList?, (any Error)?) -> Void)!
)
```

``` source
@MainActor
func contentRuleList(forIdentifier identifier: String!) async throws -> WKContentRuleList?
```

## Parameters 

`identifier`  

The identifier of the list you want.

`completionHandler`  

A completion handler block to call with the results of the search. This block has no return value and takes the following parameters:

ruleList  
The WKContentRuleList object with the specified identifier. This parameter is `nil` if the error occurs during the search.

error  
`nil` on success, or an error object if an error occurs during the search.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func contentRuleList(forIdentifier identifier: String!) async throws -> WKContentRuleList?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Accessing the Current Rule Lists

func getAvailableContentRuleListIdentifiers((([String]?) -> Void)!)

Fetches the identifiers for all rule lists in the store asynchronously.


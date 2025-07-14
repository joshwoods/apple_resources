

- WebKit
- WKContentRuleListStore
-  compileContentRuleList(forIdentifier:encodedContentRuleList:completionHandler:) 

Instance Method

# compileContentRuleList(forIdentifier:encodedContentRuleList:completionHandler:)

Compiles the specified JSON content into a new rule list and adds it to the current data store.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func compileContentRuleList(
    forIdentifier identifier: String!,
    encodedContentRuleList: String!,
    completionHandler: ((WKContentRuleList?, (any Error)?) -> Void)!
)
```

``` source
@MainActor
func compileContentRuleList(
    forIdentifier identifier: String!,
    encodedContentRuleList: String!
) async throws -> WKContentRuleList?
```

## Parameters 

`identifier`  

A unique identifier for the new list. If a list with the specified identifier already exists in the store, this method overwrites the old rule list with the new content.

`encodedContentRuleList`  

The JSON source for the new rule list. For information about how to format the JSON content, see Creating a content blocker.

`completionHandler`  

A completion handler block to call after compilation finishes. This block has no return value and takes the following parameters:

ruleList  
The WKContentRuleList object that encapsulates the compiled rules derived from the `encodedContentRuleList` parameter. This parameter is `nil` if an error occurs during compilation.

error  
`nil` on success, or an error object if a problem occurred.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Creating and Deleting Content Rule Lists

func removeContentRuleList(forIdentifier: String!, completionHandler: (((any Error)?) -> Void)!)

Removes a rule list from the current data store asynchronously.


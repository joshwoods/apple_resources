

- WebKit
- WKContentRuleListStore
-  removeContentRuleList(forIdentifier:completionHandler:) 

Instance Method

# removeContentRuleList(forIdentifier:completionHandler:)

Removes a rule list from the current data store asynchronously.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func removeContentRuleList(
    forIdentifier identifier: String!,
    completionHandler: (((any Error)?) -> Void)!
)
```

``` source
@MainActor
func removeContentRuleList(forIdentifier identifier: String!) async throws
```

## Parameters 

`identifier`  

The unique identifier for the rule list.

`completionHandler`  

A completion handler block to call after the removal of the content rule list. This block has no return value and takes the following parameter:

error  
`nil` on success, or an error object if the store encountered an error when deleting the rule list.

## Discussion

This method also removes the persistent copy of the rules stored on disk.

## See Also

### Creating and Deleting Content Rule Lists

func compileContentRuleList(forIdentifier: String!, encodedContentRuleList: String!, completionHandler: ((WKContentRuleList?, (any Error)?) -> Void)!)

Compiles the specified JSON content into a new rule list and adds it to the current data store.


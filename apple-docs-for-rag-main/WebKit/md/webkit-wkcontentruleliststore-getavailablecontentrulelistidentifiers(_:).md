

- WebKit
- WKContentRuleListStore
-  getAvailableContentRuleListIdentifiers(\_:) 

Instance Method

# getAvailableContentRuleListIdentifiers(\_:)

Fetches the identifiers for all rule lists in the store asynchronously.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
func getAvailableContentRuleListIdentifiers(_ completionHandler: (([String]?) -> Void)!)
```

``` source
@MainActor
func availableIdentifiers() async -> [String]?
```

## Parameters 

`completionHandler`  

A completion handler block to call with the results. This block has no return value and takes the following parameter:

identifierArray  
An array of strings, each of which corresponds to an identifier for a rule list in the data store. Use each string to look up the associated WKContentRuleList object. If the data store has no rule lists, the array is empty.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func availableIdentifiers() async -> [String]?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Accessing the Current Rule Lists

func lookUpContentRuleList(forIdentifier: String!, completionHandler: ((WKContentRuleList?, (any Error)?) -> Void)!)

Searches asynchronously for a specific rule list in the data store.


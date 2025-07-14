

- WebKit
- WKWebView
-  find(\_:configuration:completionHandler:) 

Instance Method

# find(\_:configuration:completionHandler:)

Searches for the specified string in the web view’s content.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOS

``` source
@MainActor @preconcurrency
func find(
    _ string: String,
    configuration: WKFindConfiguration = .init(),
    completionHandler: @escaping @MainActor (WKFindResult) -> Void
)
```

## Parameters 

`string`  

The search string to use.

`configuration`  

The search parameters. Use this object to specify whether the search is case sensitive, whether it moves forward or backward, and whether it wraps when it reaches the end of the page.

`completionHandler`  

The completion handler to call with the results of the search. This handler has no return value and takes the following parameter:

result  
The object that contains the results of the search.

## See Also

### Searching the current page’s content

func find(String, configuration: WKFindConfiguration) async throws -> WKFindResult

Searches for the specified string in the web view’s content.

class WKFindConfiguration

The configuration parameters to use when searching the contents of the web view.

class WKFindResult

An object that contains the results of searching the web view’s contents.


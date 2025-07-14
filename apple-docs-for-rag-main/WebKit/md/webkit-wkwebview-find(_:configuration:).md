

- WebKit
- WKWebView
-  find(\_:configuration:) 

Instance Method

# find(\_:configuration:)

Searches for the specified string in the web view’s content.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOS

``` source
@MainActor @preconcurrency
func find(
    _ string: String,
    configuration: WKFindConfiguration = .init()
) async throws -> WKFindResult
```

## Parameters 

`string`  

The search string to use.

`configuration`  

The search parameters. Use this object to specify whether the search is case sensitive, whether it moves forward or backward, and whether it wraps when it reaches the end of the page.

## Return Value

The object that contains the results of the search.

## See Also

### Searching the current page’s content

func find(String, configuration: WKFindConfiguration, completionHandler: (WKFindResult) -> Void)

Searches for the specified string in the web view’s content.

class WKFindConfiguration

The configuration parameters to use when searching the contents of the web view.

class WKFindResult

An object that contains the results of searching the web view’s contents.


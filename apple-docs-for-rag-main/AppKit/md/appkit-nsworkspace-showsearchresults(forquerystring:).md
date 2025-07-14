

- AppKit
- NSWorkspace
-  showSearchResults(forQueryString:) 

Instance Method

# showSearchResults(forQueryString:)

Displays a Spotlight search results window in Finder for the specified query string.

macOS 10.6+

``` source
func showSearchResults(forQueryString queryString: String) -> Bool
```

## Parameters 

`queryString`  

The string to search for.

## Return Value

true if the method communicated successfully with Finder; otherwise, false.

## Discussion

Finder becomes the active app, if possible. The user can further refine the search via the Finder user interface.

You can safely call this method from any thread of your app.


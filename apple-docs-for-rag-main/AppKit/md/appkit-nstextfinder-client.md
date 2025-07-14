

- AppKit
- NSTextFinder
-  client 

Instance Property

# client

The object that provides the target search string, find bar location, and feedback methods.

macOS 10.7+

``` source
@IBOutlet
unowned(unsafe) var client: (any NSTextFinderClient)? { get set }
```

## Discussion

The `NSTextFinder` instance class must be associated with a client object that implements the NSTextFinderClient protocol in order to function. The client is responsible for providing the string to be searched, the location for the find bar, and the methods which control feedback to the user about the search results.




- WebKit
- WebHistoryItem
-  init(urlString:title:lastVisitedTimeInterval:) Deprecated

Initializer

# init(urlString:title:lastVisitedTimeInterval:)

Initializes the receiver with a URL,`URLString`, a title specified by `title` and the last time this item was visited specified by `time` title, and time last visited.

macOS 10.3–10.14Deprecated

``` source
init!(
    urlString URLString: String!,
    title: String!,
    lastVisitedTimeInterval time: TimeInterval
)
```

## Discussion

WebKit normally creates WebHistoryItem objects for you but on occasion you might want to create an item and add it to the WebBackForwardList yourself. Note that when an instance is first initialized the strings returned by urlString and originalURLString are the same.

## See Also

### Related Documentation

WebKit Objective-C Programming Guide


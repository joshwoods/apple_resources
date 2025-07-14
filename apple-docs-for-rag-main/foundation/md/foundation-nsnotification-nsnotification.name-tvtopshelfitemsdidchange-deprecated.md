

- Foundation
- NSNotification
- NSNotification.Name
-  TVTopShelfItemsDidChange Deprecated

Type Property

# TVTopShelfItemsDidChange

A notification to post when your app’s Top Shelf content has changed.

tvOS 9.0–13.0Deprecated

``` source
static let TVTopShelfItemsDidChange: NSNotification.Name
```

Deprecated

TVTopShelfItemsDidChangeNotification has been replaced by \[TVTopShelfContentProvider topShelfContentDidChange\]

## Discussion

When the content has changed, post a new notification using the default notification center (`[NSNotificationCenter defaultCenter]`). At some point in the future, the system will fetch the new data from your extension. The notification’s parameters are ignored and should be `nil`.




- TV Services
- TVTopShelfContentProvider
-  topShelfContentDidChange() 

Type Method

# topShelfContentDidChange()

Tells the system that your top shelf content changed and requires an update.

tvOS 13.0+

``` source
class func topShelfContentDidChange()
```

## Discussion

Call this method when your top shelf content changes. This method notifies the system asynchronously and returns. You may call this method either from your app or from your Top Shelf app extension.


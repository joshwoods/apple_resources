

- Quartz
- IKImageBrowserView
-  dataSource 

Instance Property

# dataSource

Returns the data source of the receiver.

macOS 10.4+

``` source
@IBOutlet @MainActor
unowned(unsafe) var dataSource: AnyObject! { get set }
```

## Return Value

The data source (`IKImageBrowserDataSource`). The data source is not retained by the receiver.


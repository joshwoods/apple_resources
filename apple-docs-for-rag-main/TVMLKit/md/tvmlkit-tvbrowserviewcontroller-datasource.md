

- TVMLKit
- TVBrowserViewController
-  dataSource 

Instance Property

# dataSource

The object that provides data to the full-screen browser.

tvOS 13.0+

``` source
@MainActor
weak var dataSource: (any TVBrowserViewControllerDataSource)? { get set }
```

## See Also

### Providing the Browser’s Data

protocol TVBrowserViewControllerDataSource

Methods adopted by the object you use to represent the browser view.


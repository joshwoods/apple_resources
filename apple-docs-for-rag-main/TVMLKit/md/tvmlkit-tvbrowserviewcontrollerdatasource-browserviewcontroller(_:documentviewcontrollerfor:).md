

- TVMLKit
- TVBrowserViewControllerDataSource
-  browserViewController(\_:documentViewControllerFor:) 

Instance Method

# browserViewController(\_:documentViewControllerFor:)

Provides the document view controller to be used for a particular child of the full-screen browser.

tvOS 13.0+

``` source
func browserViewController(
    _ browserViewController: TVBrowserViewController,
    documentViewControllerFor viewElement: TVViewElement
) -> TVDocumentViewController?
```

**Required**


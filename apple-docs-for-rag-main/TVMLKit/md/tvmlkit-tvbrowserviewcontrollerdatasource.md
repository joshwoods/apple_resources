

- TVMLKit
-  TVBrowserViewControllerDataSource 

Protocol

# TVBrowserViewControllerDataSource

Methods adopted by the object you use to represent the browser view.

tvOS 13.0+

``` source
protocol TVBrowserViewControllerDataSource : NSObjectProtocol
```

## Overview

Use the data source to provide a document to the browser.

## Topics

### Providing Data

func browserViewController(TVBrowserViewController, documentViewControllerFor: TVViewElement) -> TVDocumentViewController?

Provides the document view controller to be used for a particular child of the full-screen browser.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Providing the Browser’s Data

var dataSource: (any TVBrowserViewControllerDataSource)?

The object that provides data to the full-screen browser.


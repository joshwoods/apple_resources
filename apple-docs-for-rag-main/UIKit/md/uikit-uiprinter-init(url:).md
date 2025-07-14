

- UIKit
- UIPrinter
-  init(url:) 

Initializer

# init(url:)

Creates and returns a printer with the specified location.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(url: URL)
```

## Parameters 

`url`  

A URL that identifies the location of the printer on your network.

## Return Value

A printer object representing the specified printer or `nil` if there was a problem initializing the object.

## Discussion

Use this method to create printer objects for printers whose address you already know. The printer does not need to be online or available when you call this method. The URL you specify is stored in the returned object so that you can contact the printer later using the contactPrinter(_:) method.


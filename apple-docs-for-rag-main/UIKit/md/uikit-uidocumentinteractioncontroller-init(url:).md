

- UIKit
- UIDocumentInteractionController
-  init(url:) 

Initializer

# init(url:)

Creates a document interaction controller with the specified URL.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(url: URL)
```

## Parameters 

`url`  

A URL that specifies the location of the desired document. This parameter is retained. It can be changed later by modifying the url property.

## Return Value

A new document interaction controller object.


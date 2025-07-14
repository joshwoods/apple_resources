

- UIKit
- UIScene
- UIScene.OpenURLOptions
-  openInPlace 

Instance Property

# openInPlace

A Boolean value that indicates whether you should open the URL at its current location instead of copying it to your app’s container.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var openInPlace: Bool { get }
```

## Discussion

When the value of this property is false, copy the document to your app’s container before opening the file. When the value of this property is true, open the existing URL in its current location.


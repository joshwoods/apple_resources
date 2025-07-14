

- UIKit
- UIContextMenuConfiguration
-  identifier 

Instance Property

# identifier

The unique identifier for this configuration object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var identifier: any NSCopying { get }
```

## Discussion

If you did not provide an identifier when creating this object, UIKit assigns a new UUID object to this property.


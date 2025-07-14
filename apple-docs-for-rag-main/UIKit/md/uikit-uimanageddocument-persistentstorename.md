

- UIKit
- UIManagedDocument
-  persistentStoreName 

Type Property

# persistentStoreName

Returns the name for the persistent store file inside the document’s file package.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class var persistentStoreName: String { get }
```

## Return Value

The name for the persistent store file inside the document’s file package.

## Discussion

This path component is appended to the document URL provided by UIDocument. The default name is `persistentStore`.


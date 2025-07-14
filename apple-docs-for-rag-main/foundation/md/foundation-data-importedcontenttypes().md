

- Foundation
- Data
-  importedContentTypes() 

Instance Method

# importedContentTypes()

Content types supported by a given value’s `Transferable` conformance for import (like drop or paste).

FoundationCoreTransferableiOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func importedContentTypes() -> [UTType]
```

## Discussion

Returns a list of all content types available for import. The default implementation of this function is available to all types that conform to `Transferable` protocol.


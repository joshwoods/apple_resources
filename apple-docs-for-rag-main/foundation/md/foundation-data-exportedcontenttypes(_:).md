

- Foundation
- Data
-  exportedContentTypes(\_:) 

Instance Method

# exportedContentTypes(\_:)

Content types supported by a given value’s `Transferable` conformance for export (like drag or copy).

FoundationCoreTransferableiOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
func exportedContentTypes(_ visibility: TransferRepresentationVisibility = .all) -> [UTType]
```

## Parameters 

`visibility`  

Desired visibility level for the returned content types. Defaults to `.all`.

## Discussion

Returns a list of all content types available for export in the type’s `Transferable` conformance, except for those that are not supported by this specific value. For example, if an `exportingCondition` for some representation evaluates to `false`, this representation isn’t included.

The default implementation of this function is available to all types that conform to `Transferable` protocol.


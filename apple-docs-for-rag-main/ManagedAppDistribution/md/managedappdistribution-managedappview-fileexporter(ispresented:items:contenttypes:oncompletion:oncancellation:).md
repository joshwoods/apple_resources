

- ManagedAppDistribution
- ManagedAppView
-  fileExporter(isPresented:items:contentTypes:onCompletion:onCancellation:) 

Instance Method

# fileExporter(isPresented:items:contentTypes:onCompletion:onCancellation:)

Presents a system interface allowing the user to export a collection of items to files on disk.

ManagedAppDistributionSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
nonisolated
func fileExporter(
    isPresented: Binding,
    items: C,
    contentTypes: [UTType] = [],
    onCompletion: @escaping (Result) -> Void,
    onCancellation: @escaping () -> Void = { }
) -> some View where C : Collection, T : Transferable, T == C.Element
```

## Parameters 

`isPresented`  

A binding to whether the interface should be shown.

`items`  

Collection of values to be saved on disk.

`contentTypes`  

The content types to use for the exported file. If empty, SwiftUI uses the content types from the `transferRepresentation` property provided for `Transferable` conformance.

`allowsOtherContentTypes`  

A Boolean value that indicates if the users are allowed to save the files with a different file extension than specified by the `contentType` property.

`onCompletion`  

A callback that will be invoked when the operation has has succeeded or failed.

`onCancellation`  

A callback that will be invoked if the operation was cancelled.

## Discussion

In order for the interface to appear `isPresented` must be set to `true`. When the operation is finished, `isPresented` will be set to `false` before `onCompletion` is called. If the user cancels the operation, `isPresented` will be set to `false` and `onCompletion` will not be called.


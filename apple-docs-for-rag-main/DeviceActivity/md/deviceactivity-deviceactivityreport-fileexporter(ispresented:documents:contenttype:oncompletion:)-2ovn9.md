

- DeviceActivity
- DeviceActivityReport
-  fileExporter(isPresented:documents:contentType:onCompletion:) 

Instance Method

# fileExporter(isPresented:documents:contentType:onCompletion:)

Presents a system interface for exporting a collection of reference type documents to files on disk.

DeviceActivitySwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
nonisolated
func fileExporter(
    isPresented: Binding,
    documents: C,
    contentType: UTType,
    onCompletion: @escaping (Result) -> Void
) -> some View where C : Collection, C.Element : ReferenceFileDocument
```

## Parameters 

`isPresented`  

A binding to whether the interface should be shown.

`documents`  

The collection of in-memory documents to export.

`contentType`  

The content type to use for the exported file.

`onCompletion`  

A callback that will be invoked when the operation has has succeeded or failed.

`result`  

A `Result` indicating whether the operation succeeded or failed.

## Discussion

In order for the interface to appear, both `isPresented` must be `true` and `documents` must not be empty. When the operation is finished, `isPresented` will be set to `false` before `onCompletion` is called. If the user cancels the operation, `isPresented` will be set to `false` and `onCompletion` will not be called.

The `contentType` provided must be included within the document type’s `writableContentTypes`, otherwise the first valid writable content type will be used instead.


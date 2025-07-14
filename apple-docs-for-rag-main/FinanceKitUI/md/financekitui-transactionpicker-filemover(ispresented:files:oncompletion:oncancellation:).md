

- FinanceKitUI
- TransactionPicker
-  fileMover(isPresented:files:onCompletion:onCancellation:) 

Instance Method

# fileMover(isPresented:files:onCompletion:onCancellation:)

Presents a system dialog for allowing the user to move a collection of existing files to a new location.

FinanceKitUISwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
nonisolated
func fileMover(
    isPresented: Binding,
    files: C,
    onCompletion: @escaping (Result) -> Void,
    onCancellation: @escaping () -> Void
) -> some View where C : Collection, C.Element == URL
```

## Parameters 

`isPresented`  

A binding to whether the dialog should be shown.

`files`  

A collection of URLs for the files to be moved.

`onCompletion`  

A callback that will be invoked when the operation has succeeded or failed. The `result` indicates whether the operation succeeded or failed. To access the received URLs, call `startAccessingSecurityScopedResource`. When the access is no longer required, call `stopAccessingSecurityScopedResource`.

`onCancellation`  

A callback that will be invoked if the user cancels the operation.

## Discussion

Note

This dialog provides security-scoped URLs. Call the `startAccessingSecurityScopedResource` method to access or bookmark the URLs, and the `stopAccessingSecurityScopedResource` method to release the access.

For example, a button that allows the user to move files might look like this:

```
  struct MoveFilesButton: View {
      @Binding var files: [URL]
      @State private var showFileMover = false
      var onCompletion: (URL) -> Void
      var onCancellation: (() -> Void)?

      var body: some View {
          Button {
              showFileMover = true
          } label: {
              Label("Choose destination", systemImage: "folder.circle")
          }
          .fileMover(isPresented: $showFileMover, files: files) { result in
              switch result {
              case .success(let urls):
                  urls.forEach { url in
                      guard url.startAccessingSecurityScopedResource() else {
                          return
                      }
                      onCompletion(url)
                      url.stopAccessingSecurityScopedResource()
                  }
              case .failure(let error):
                  print(error)
                  // handle error
              }
          } onCancellation: {
              onCancellation?()
          }
      }
  }
```




- SwiftUI
- View
-  photosPicker(isPresented:selection:maxSelectionCount:selectionBehavior:matching:preferredItemEncoding:) 

Instance Method

# photosPicker(isPresented:selection:maxSelectionCount:selectionBehavior:matching:preferredItemEncoding:)

Presents a Photos picker that selects a collection of `PhotosPickerItem`.

PhotosUISwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+watchOS 9.0+

``` source
nonisolated
func photosPicker(
    isPresented: Binding,
    selection: Binding,
    maxSelectionCount: Int? = nil,
    selectionBehavior: PhotosPickerSelectionBehavior = .default,
    matching filter: PHPickerFilter? = nil,
    preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy = .automatic
) -> some View
```

## Parameters 

`isPresented`  

The binding to whether the Photos picker should be shown.

`selection`  

All items being shown and selected in the Photos picker.

`maxSelectionCount`  

The maximum number of items that can be selected. Default is `nil`. Setting it to `nil` means maximum supported by the system.

`selectionBehavior`  

The selection behavior of the Photos picker. Default is `.default`.

`filter`  

Types of items that can be shown. Default is `nil`. Setting it to `nil` means all supported types can be shown.

`preferredItemEncoding`  

The encoding disambiguation policy of selected items. Default is `.automatic`. Setting it to `.automatic` means the best encoding determined by the system will be used.

## Discussion

The user explicitly grants access only to items they choose, so photo library access authorization is not needed.

## See Also

### Selecting photos

@MainActor @preconcurrency struct PhotosPicker&lt;Label> where Label : View

A view that displays a Photos picker for choosing assets from the photo library.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;PhotosPickerItem?>, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy) -> some View

Presents a Photos picker that selects a `PhotosPickerItem`.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;PhotosPickerItem?>, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy, photoLibrary: PHPhotoLibrary) -> some View

Presents a Photos picker that selects a `PhotosPickerItem` from a given photo library.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;[PhotosPickerItem]>, maxSelectionCount: Int?, selectionBehavior: PhotosPickerSelectionBehavior, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy, photoLibrary: PHPhotoLibrary) -> some View

Presents a Photos picker that selects a collection of `PhotosPickerItem` from a given photo library.

func photosPickerAccessoryVisibility(Visibility, edges: Edge.Set) -> some View

Sets the accessory visibility of the Photos picker. Accessories include anything between the content and the edge, like the navigation bar or the sidebar.

func photosPickerDisabledCapabilities(PHPickerCapabilities) -> some View

Disables capabilities of the Photos picker.

func photosPickerStyle(PhotosPickerStyle) -> some View

Sets the mode of the Photos picker.


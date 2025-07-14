

- SwiftUI
- View
-  photosPickerAccessoryVisibility(\_:edges:) 

Instance Method

# photosPickerAccessoryVisibility(\_:edges:)

Sets the accessory visibility of the Photos picker. Accessories include anything between the content and the edge, like the navigation bar or the sidebar.

PhotosUISwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
nonisolated
func photosPickerAccessoryVisibility(
    _ visibility: Visibility,
    edges: Edge.Set = .all
) -> some View
```

## Parameters 

`edges`  

The accessory visibility to apply.

`edges`  

One or more of the available edges.

## Return Value

A Photos picker with the specified accessory visibility.

## See Also

### Selecting photos

@MainActor @preconcurrency struct PhotosPicker&lt;Label> where Label : View

A view that displays a Photos picker for choosing assets from the photo library.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;PhotosPickerItem?>, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy) -> some View

Presents a Photos picker that selects a `PhotosPickerItem`.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;PhotosPickerItem?>, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy, photoLibrary: PHPhotoLibrary) -> some View

Presents a Photos picker that selects a `PhotosPickerItem` from a given photo library.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;[PhotosPickerItem]>, maxSelectionCount: Int?, selectionBehavior: PhotosPickerSelectionBehavior, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy) -> some View

Presents a Photos picker that selects a collection of `PhotosPickerItem`.

func photosPicker(isPresented: Binding&lt;Bool>, selection: Binding&lt;[PhotosPickerItem]>, maxSelectionCount: Int?, selectionBehavior: PhotosPickerSelectionBehavior, matching: PHPickerFilter?, preferredItemEncoding: PhotosPickerItem.EncodingDisambiguationPolicy, photoLibrary: PHPhotoLibrary) -> some View

Presents a Photos picker that selects a collection of `PhotosPickerItem` from a given photo library.

func photosPickerDisabledCapabilities(PHPickerCapabilities) -> some View

Disables capabilities of the Photos picker.

func photosPickerStyle(PhotosPickerStyle) -> some View

Sets the mode of the Photos picker.


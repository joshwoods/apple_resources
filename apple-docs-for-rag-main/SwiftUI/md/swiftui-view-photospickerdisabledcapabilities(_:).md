

- SwiftUI
- View
-  photosPickerDisabledCapabilities(\_:) 

Instance Method

# photosPickerDisabledCapabilities(\_:)

Disables capabilities of the Photos picker.

PhotosUISwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+

``` source
nonisolated
func photosPickerDisabledCapabilities(_ disabledCapabilities: PHPickerCapabilities) -> some View
```

## Parameters 

`disabledCapabilities`  

One or more of the available capabilities.

## Return Value

A Photos picker with specified capabilities that are disabled.

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

func photosPickerAccessoryVisibility(Visibility, edges: Edge.Set) -> some View

Sets the accessory visibility of the Photos picker. Accessories include anything between the content and the edge, like the navigation bar or the sidebar.

func photosPickerStyle(PhotosPickerStyle) -> some View

Sets the mode of the Photos picker.


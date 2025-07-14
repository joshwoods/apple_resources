

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  navigationTitle(\_:) 

Instance Method

# navigationTitle(\_:)

Configures the view’s title for purposes of navigation, using a string binding.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func navigationTitle(_ title: Binding) -> some View
```

## Parameters 

`title`  

The text of the title.

## Discussion

In iOS, iPadOS, and macOS, this allows editing the navigation title when the title is displayed in the toolbar.

Refer to the doc:Configure-Your-Apps-Navigation-Titles article for more information on navigation title modifiers.


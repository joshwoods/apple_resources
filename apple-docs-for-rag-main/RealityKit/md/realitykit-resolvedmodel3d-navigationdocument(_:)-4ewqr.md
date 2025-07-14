

- RealityKit
- ResolvedModel3D
-  navigationDocument(\_:) 

Instance Method

# navigationDocument(\_:)

Configures the view’s document for purposes of navigation.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
nonisolated
func navigationDocument(_ url: URL) -> some View
```

## Parameters 

`document`  

The URL content associated to the navigation title.

`preview`  

The preview of the document to use when sharing.

## Discussion

In iOS, iPadOS, this populates the title menu with a header previewing the document. In macOS, this populates a proxy icon.

Refer to the doc:Configure-Your-Apps-Navigation-Titles article for more information on navigation document modifiers.


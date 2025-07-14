

- RealityKit
- ObjectCaptureView
-  navigationDocument(\_:) 

Instance Method

# navigationDocument(\_:)

Configures the view’s document for purposes of navigation.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
nonisolated
func navigationDocument(_ document: D) -> some View where D : Transferable
```

## Parameters 

`document`  

The transferable content associated to the navigation title.

## Discussion

In iOS, iPadOS, this populates the title menu with a header previewing the document. In macOS, this populates a proxy icon.

Refer to the doc:Configure-Your-Apps-Navigation-Titles article for more information on navigation document modifiers.


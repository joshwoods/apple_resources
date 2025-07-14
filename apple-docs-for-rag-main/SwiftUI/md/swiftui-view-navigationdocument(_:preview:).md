

- SwiftUI
- View
-  navigationDocument(\_:preview:) 

Instance Method

# navigationDocument(\_:preview:)

Configures the view’s document for purposes of navigation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func navigationDocument(
    _ document: D,
    preview: SharePreview
) -> some View where D : Transferable, I1 : Transferable, I2 : Transferable
```

Show all declarations

## Parameters 

`document`  

The transferable content associated to the navigation title.

`preview`  

The preview of the document to use when sharing.

## Discussion

In iOS, iPadOS, this populates the title menu with a header previewing the document. In macOS, this populates a proxy icon.

Refer to the Configure your apps navigation titles article for more information on navigation document modifiers.

## See Also

### Setting titles for navigation content

func navigationTitle(_:)

Configures the view’s title for purposes of navigation, using a string binding.

func navigationSubtitle(_:)

Configures the view’s subtitle for purposes of navigation.

func navigationDocument(_:)

Configures the view’s document for purposes of navigation.


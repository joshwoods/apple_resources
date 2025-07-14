

- FinanceKitUI
- TransactionPicker
-  navigationDocument(\_:preview:) 

Instance Method

# navigationDocument(\_:preview:)

Configures the view’s document for purposes of navigation.

FinanceKitUISwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+watchOS 9.0+

``` source
nonisolated
func navigationDocument(
    _ document: D,
    preview: SharePreview
) -> some View where D : Transferable, I : Transferable
```

## Parameters 

`document`  

The transferable content associated to the navigation title.

`preview`  

The preview of the document to use when sharing.

## Discussion

In iOS, iPadOS, this populates the title menu with a header previewing the document. In macOS, this populates a proxy icon.

Refer to the doc:Configure-Your-Apps-Navigation-Titles article for more information on navigation document modifiers.


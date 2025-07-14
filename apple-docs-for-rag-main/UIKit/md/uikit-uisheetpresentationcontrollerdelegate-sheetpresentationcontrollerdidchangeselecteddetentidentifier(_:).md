

- UIKit
- UISheetPresentationControllerDelegate
-  sheetPresentationControllerDidChangeSelectedDetentIdentifier(\_:) 

Instance Method

# sheetPresentationControllerDidChangeSelectedDetentIdentifier(\_:)

Provides an opportunity to respond after the sheet presentation controller’s selected detent changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor
optional func sheetPresentationControllerDidChangeSelectedDetentIdentifier(_ sheetPresentationController: UISheetPresentationController)
```

## Parameters 

`sheetPresentationController`  

The sheet presentation controller whose detent changes.

## Discussion

Implement this method if you want to perform changes in response to the user resizing a sheet to a new detent.

The system calls this method after a sheet’s selectedDetentIdentifier changes in response to user interaction. The system doesn’t call this after you change selectedDetentIdentifier programmatically.


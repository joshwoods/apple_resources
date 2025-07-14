

- UIKit
- UITextFormattingViewController
-  UITextFormattingViewController.Delegate 

Protocol

# UITextFormattingViewController.Delegate

iOS 18.0+iPadOS 18.0+

``` source
@MainActor
protocol Delegate : AnyObject
```

## Topics

### Instance Methods

func textFormattingDidFinish(UITextFormattingViewController)

**Required** Default implementation provided.

func textFormattingViewController(UITextFormattingViewController, didChangeValue: UITextFormattingViewController.ChangeValue)

**Required**

func textFormattingViewController(UITextFormattingViewController, shouldPresentColorPicker: UIColorPickerViewController) -> Bool

**Required** Default implementation provided.

func textFormattingViewController(UITextFormattingViewController, shouldPresentFontPicker: UIFontPickerViewController) -> Bool

**Required** Default implementation provided.


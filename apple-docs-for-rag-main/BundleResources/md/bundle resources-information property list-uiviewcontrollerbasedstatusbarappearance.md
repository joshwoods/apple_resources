

- Bundle Resources
- Information Property List
-  UIViewControllerBasedStatusBarAppearance 

Property List Key

# UIViewControllerBasedStatusBarAppearance

A Boolean value that indicates whether the system bases the appearance of the status bar on the style preferred by the current view controller.

iOS 7.0+iPadOS 7.0+

## Details 

Name  
View controller-based status bar appearance

Type  

boolean

## Discussion

If this key is `YES`, the system uses the current view controller’s preferred status bar style. If this key is `NO`, it uses the status bar style of the UIApplication object. The default value is `YES`.

## See Also

### Status bar

UIStatusBarHidden

A Boolean value that indicates whether the system initially hides the status bar when the app launches.

**Name:** Status bar is initially hidden

UIStatusBarStyle

The style of the status bar as the app launches.

**Name:** Status bar style

UIStatusBarTintParameters

The status bar tint.

**Name:** Status bar tinting parameters


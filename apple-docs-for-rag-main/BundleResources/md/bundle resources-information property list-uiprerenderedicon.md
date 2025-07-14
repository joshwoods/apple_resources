

- Bundle Resources
- Information Property List
-  UIPrerenderedIcon 

Property List Key

# UIPrerenderedIcon

A Boolean value that indicates whether the app’s icon contains a shine effect.

iOS 2.0+iPadOS 2.0+tvOS 9.0+watchOS 2.0+

## Details 

Name  
Icon already includes gloss effects

Type  

boolean

## Discussion

If `YES`, the system doesn’t apply a shine effect to the app icon; otherwise, it does. If your app icon already has a shine, set this key to `YES` to prevent the system from applying the same effect again. The default value is `NO`.

## See Also

### Icons

CFBundleIcons

Information about all of the icons used by the app.

**Name:** Icon files (iOS 5)

CFBundleIconFiles

The names of the bundle’s icon image files.

**Name:** Icon files

CFBundleIconFile

The file containing the bundle’s icon.

**Name:** Icon file

CFBundleIconName

The name of the asset that represents the app icon.

**Name:** Icon Name


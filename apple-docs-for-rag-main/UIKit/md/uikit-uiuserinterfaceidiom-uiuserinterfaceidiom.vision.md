

- UIKit
- UIUserInterfaceIdiom
-  UIUserInterfaceIdiom.vision 

Case

# UIUserInterfaceIdiom.vision

An interface designed for visionOS and Apple Vision Pro.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
case vision
```

## Discussion

If your app has existing code that runs in the UIUserInterfaceIdiom.pad idiom, you might want to reuse the same code in the UIUserInterfaceIdiom.vision idiom. The following code shows how to check for these idioms:

```
if idiom == .pad || idiom == .vision {
   // Code to run in the iPad or Apple Vision Pro idioms.
} else { 
   // Code to run in other idioms.
}
```

## See Also

### Idioms

case unspecified

An unspecified idiom.

case phone

An interface designed for iPhone and iPod touch.

case pad

An interface designed for iPad.

case tv

An interface designed for tvOS and Apple TV.

case carPlay

An interface designed for an in-car experience.

case mac

An interface designed for the Mac.


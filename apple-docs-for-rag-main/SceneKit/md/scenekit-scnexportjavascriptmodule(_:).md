

- SceneKit
-  SCNExportJavaScriptModule(\_:) 

Function

# SCNExportJavaScriptModule(\_:)

Makes SceneKit classes and global constants available to the specified JavaScript context.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func SCNExportJavaScriptModule(_ context: JSContext)
```

## Discussion

By controlling SceneKit using JavaScript code supplied at run time, you can enable rapid development for parts of your game or app. For example, a designer can easily experiment with visual effects or game-character behaviors without needing to compile and deploy your complete Xcode project.

This function exports all SceneKit classes and global constants, and all methods and properties on those classes, to JavaScript using the rules defined in the JSExport protocol. For example, the JavaScript code below performs various operations on a SceneKit node:

```
```

For SceneKit APIs that involve vectors and matrices, use JavaScript object syntax to define those values in terms of their elements:

```
```

SceneKit also exports the following special JavaScript objects and functions:

| Objective-C / Swift class | JavaScript constructor |
|----|----|
| NSColor / UIColor | `SCNColor.color(r,g,b,a)` |
| NSImage / UIImage | `SCNImage.imageWithURL(aURL)` |
|  | `SCNImage.imageWithPath(aPath)` |
| CABasicAnimation | `CABasicAnimation.animationWithKeyPath(aPath)` |
| CAKeyframeAnimation | `CAKeyframeAnimation.animationWithKeyPath(aPath)` |
| CAAnimationGroup | `new CAAnimationGroup()` |
| CAMediaTimingFunction | `CAMediaTimingFunction.functionWithName(name)` |


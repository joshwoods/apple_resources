

- UIKit
- UITextInputTraits
-  writingToolsBehavior 

Instance Property

# writingToolsBehavior

The writing tools experience to support in the current view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.4+

``` source
@MainActor
optional var writingToolsBehavior: UIWritingToolsBehavior { get set }
```

## Mentioned in 

Customizing Writing Tools behavior for UIKit views

## Discussion

Use this property to specify the type of experience to display when someone engages writing tools for a text input view. The system does its best to provide the requested UI, but might offer a more limited experience if required capabilities aren’t available. The default value of this property is UIWritingToolsBehavior.default, which lets the system choose the most appropriate experience for the current device.

Set the value of this property to UIWritingToolsBehavior.none if you want to prevent someone from using the writing tools with your view.

## See Also

### Configuring the writing tools experience

enum UIWritingToolsBehavior

Constants that specify the writing tools experience for the underlying view.


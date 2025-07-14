

- UIKit
- UIWritingToolsCoordinator
-  preferredResultOptions 

Instance Property

# preferredResultOptions

The type of content you allow Writing Tools to generate for your custom text view.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+visionOS 2.4+

``` source
@MainActor
var preferredResultOptions: UIWritingToolsResultOptions { get set }
```

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Discussion

Writing Tools can create plain text or rich text, and it can format text using lists or tables as needed. If your view doesn’t support specific types of content, specify the types you do support in this property. The default value of this property is `UIWritingToolsResultOptions/default`, which lets the system determine the type of content to generate.

## See Also

### Configuring the experience

var preferredBehavior: UIWritingToolsBehavior

The level of Writing Tools support you want the system to provide for your view.

var behavior: UIWritingToolsBehavior

The actual level of Writing Tools support the system provides for your view.

var resultOptions: UIWritingToolsResultOptions

The type of content the system generates for your custom text view.


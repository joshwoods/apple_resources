

- CarPlay
- CPInterfaceController
-  presentedTemplate 

Instance Property

# presentedTemplate

The interface controller’s current modal template.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var presentedTemplate: CPTemplate? { get }
```

## See Also

### Displaying Templates Modally

func presentTemplate(CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Presents a template modally.

func dismissTemplate(animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Dismisses a modal template.




- CarPlay
- CPInterfaceControllerDelegate
-  templateDidDisappear(\_:animated:) 

Instance Method

# templateDidDisappear(\_:animated:)

Tells the delegate that the template did disappear from the screen.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func templateDidDisappear(
    _ aTemplate: CPTemplate,
    animated: Bool
)
```

## Parameters 

`animated`  

A Boolean value indicating whether the system animated the disappearance of the template.

## See Also

### Handling Display Events

func templateWillAppear(CPTemplate, animated: Bool)

Tells the delegate that the template will appear onscreen.

func templateDidAppear(CPTemplate, animated: Bool)

Tells the delegate that the template did appear onscreen.

func templateWillDisappear(CPTemplate, animated: Bool)

Tells the delegate that the template will disappear from the screen.


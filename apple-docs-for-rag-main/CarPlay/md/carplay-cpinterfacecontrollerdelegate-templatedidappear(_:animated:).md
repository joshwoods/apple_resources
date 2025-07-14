

- CarPlay
- CPInterfaceControllerDelegate
-  templateDidAppear(\_:animated:) 

Instance Method

# templateDidAppear(\_:animated:)

Tells the delegate that the template did appear onscreen.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func templateDidAppear(
    _ aTemplate: CPTemplate,
    animated: Bool
)
```

## Parameters 

`animated`  

A Boolean value indicating whether the system animated the presentation of the template.

## See Also

### Handling Display Events

func templateWillAppear(CPTemplate, animated: Bool)

Tells the delegate that the template will appear onscreen.

func templateWillDisappear(CPTemplate, animated: Bool)

Tells the delegate that the template will disappear from the screen.

func templateDidDisappear(CPTemplate, animated: Bool)

Tells the delegate that the template did disappear from the screen.


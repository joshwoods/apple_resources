

- CarPlay
- CPInterfaceControllerDelegate
-  templateWillAppear(\_:animated:) 

Instance Method

# templateWillAppear(\_:animated:)

Tells the delegate that the template will appear onscreen.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func templateWillAppear(
    _ aTemplate: CPTemplate,
    animated: Bool
)
```

## Parameters 

`animated`  

A Boolean value indicating whether the system animates the presentation of the template.

## See Also

### Handling Display Events

func templateDidAppear(CPTemplate, animated: Bool)

Tells the delegate that the template did appear onscreen.

func templateWillDisappear(CPTemplate, animated: Bool)

Tells the delegate that the template will disappear from the screen.

func templateDidDisappear(CPTemplate, animated: Bool)

Tells the delegate that the template did disappear from the screen.


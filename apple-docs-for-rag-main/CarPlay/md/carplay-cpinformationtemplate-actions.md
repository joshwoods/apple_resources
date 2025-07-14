

- CarPlay
- CPInformationTemplate
-  actions 

Instance Property

# actions

The actions that the template displays.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var actions: [CPTextButton] { get set }
```

## Discussion

Assign a new array to this property to update the actions that the template displays. The template can display three actions maximum. If the array contains more actions, the template uses only the first three.


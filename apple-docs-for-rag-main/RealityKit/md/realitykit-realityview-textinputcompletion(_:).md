

- RealityKit
- RealityView
-  textInputCompletion(\_:) 

Instance Method

# textInputCompletion(\_:)

Associates a fully formed string with the value of this view when used as a text input suggestion

RealityKitSwiftUImacOS 15.0+

``` source
nonisolated
func textInputCompletion(_ completion: String) -> some View
```

## Parameters 

`text`  

A string to use as the view’s completion.

## Discussion

Use this method to associate a fully formed string with a view that is within a text input suggestion list context. The system uses this value when the view is selected to replace the partial text being currently edited of the associated text field.

```
TextField("Location", text: $addressText)
    .textInputSuggestions(isEnabled: true) {
        Text("The Fillmore")
            .textInputCompletion("1805 Geary Blvd, San Francisco")
        Text("The Catalyst")
            .textInputCompletion("1011 Pacific Ave, Santa Cruz")
        Text("Rio Theatre")
            .textInputCompletion("1205 Soquel Ave, Santa Cruz")
    }
```


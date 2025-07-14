

- Objective-C Runtime
- NSObject
-  shouldEnableAction(for:identifier:) 

Instance Method

# shouldEnableAction(for:identifier:)

Sent to the delegate to determine whether the action should be enabled.

macOS

``` source
func shouldEnableAction(
    for person: ABPerson!,
    identifier: String!
) -> Bool
```

## Parameters 

`person`  

The person on which the action will be taken.

`identifier`  

The unique identifier of the selected value.

## Return Value

YES if the action is applicable; otherwise, NO.

## Discussion

If the property returned by actionProperty() is a multivalue property, `identifier` contains the unique identifier of the value selected.




- Objective-C Runtime
- NSObject
-  performAction(for:identifier:) 

Instance Method

# performAction(for:identifier:)

Sent to the delegate to perform the action.

macOS

``` source
func performAction(
    for person: ABPerson!,
    identifier: String!
)
```

## Parameters 

`person`  

The person on which the action will be taken.

`identifier`  

The unique identifier of the selected value.

## Discussion

If the property returned by actionProperty() is a multivalue property, `identifier` contains the unique identifier of the value selected. The person being displayed in the Address Book application’s card view when the rollover menu is accesses is passed as `person`.


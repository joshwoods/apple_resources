

- Objective-C Runtime
- NSObject
-  title(for:identifier:) 

Instance Method

# title(for:identifier:)

Sent to the delegate to request the title of the menu item for the action.

macOS

``` source
func title(
    for person: ABPerson!,
    identifier: String!
) -> String!
```

## Parameters 

`person`  

The person on which the action will be taken.

`identifier`  

The unique identifier of the value for which the menu item will be displayed.

## Return Value

The title of the menu item for the action.

## Discussion

If the property returned by actionProperty() is a multivalue property, `identifier` contains the unique identifier of the value selected.




- AppKit
- NSRuleEditor
-  displayValues(forRow:) 

Instance Method

# displayValues(forRow:)

Returns the chosen values for a given row.

macOS

``` source
@MainActor
func displayValues(forRow row: Int) -> [Any]
```

## Parameters 

`row`  

The index of a row in the receiver.

## Return Value

The chosen values (strings, views, or menu items) for row `row`.

## Discussion

The values returned are the same as those returned from the delegate’s ruleEditor(_:displayValueForCriterion:inRow:) method.

## See Also

### Providing Data

func reloadCriteria()

Instructs the receiver to refetch criteria from its delegate.

func setCriteria([Any], andDisplayValues: [Any], forRowAt: Int)

Modifies the row at a given index to contain the given items and values.

func criteria(forRow: Int) -> [Any]

Returns the currently chosen items for a given row.


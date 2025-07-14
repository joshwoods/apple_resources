

- AppKit
- NSRuleEditor
-  criteria(forRow:) 

Instance Method

# criteria(forRow:)

Returns the currently chosen items for a given row.

macOS

``` source
@MainActor
func criteria(forRow row: Int) -> [Any]
```

## Parameters 

`row`  

The index of a row in the receiver.

## Return Value

The currently chosen items for row `row`.

## Discussion

The items returned are the same as those returned by calling the delegate’s ruleEditor(_:child:forCriterion:with:) method once for each item in the row.

## See Also

### Providing Data

func reloadCriteria()

Instructs the receiver to refetch criteria from its delegate.

func setCriteria([Any], andDisplayValues: [Any], forRowAt: Int)

Modifies the row at a given index to contain the given items and values.

func displayValues(forRow: Int) -> [Any]

Returns the chosen values for a given row.


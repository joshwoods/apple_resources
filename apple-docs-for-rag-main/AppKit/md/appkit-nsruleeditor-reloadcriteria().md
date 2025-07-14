

- AppKit
- NSRuleEditor
-  reloadCriteria() 

Instance Method

# reloadCriteria()

Instructs the receiver to refetch criteria from its delegate.

macOS

``` source
@MainActor
func reloadCriteria()
```

## Discussion

You can use this method to indicate that the available criteria may have changed and should be refetched from the delegate and the popups recalculated. If any item in a given row is “orphaned” (that is, is no longer reported as a child of its previous parent), its criteria and display values are set to valid choices.

## See Also

### Providing Data

func setCriteria([Any], andDisplayValues: [Any], forRowAt: Int)

Modifies the row at a given index to contain the given items and values.

func criteria(forRow: Int) -> [Any]

Returns the currently chosen items for a given row.

func displayValues(forRow: Int) -> [Any]

Returns the chosen values for a given row.


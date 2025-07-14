

- Address Book
- ABPeoplePickerView
-  selectedIdentifiers(for:) 

Instance Method

# selectedIdentifiers(for:)

Returns the identifiers of the selected values in a multivalue property.

macOS 10.3+

``` source
@MainActor
func selectedIdentifiers(for person: ABPerson!) -> [Any]!
```

## Parameters 

`person`  

The person whose identifiers for selected values will be returned.

## Discussion

Returns `nil` if the property displayed is a single-value property, or if the selected value is not a property of `person`.

The selectedRecords property returns all of the person records that were unified to display the selected records, which can require some extra care in passing the correct person record.

## See Also

### Selecting Groups and Records

var allowsGroupSelection: Bool

A Boolean value that specifies whether the user can select entire groups in the group column.

var allowsMultipleSelection: Bool

A Boolean value that specifies whether multiple groups, records, or values of multivalue properties can be selected at a time.

func deselectAll(Any!)

Deselects all selected groups, records, and values in multivalue properties.

func deselect(ABGroup!)

Deselects a group selected in the group list.

func deselectIdentifier(String!, for: ABPerson!)

Deselects a value selected in a multivalue property.

func deselect(ABRecord!)

Deselects a record selected in the record list.

var selectedGroups: [Any]!

The groups selected in the group list. (read-only)

var selectedRecords: [Any]!

The selection in the records list. (read-only)

func selectedValues() -> [Any]!

Returns an array of all the values selected in the displayed multivalue property.

func select(ABGroup!, byExtendingSelection: Bool)

Selects a group or a set of groups in the group list.

func selectIdentifier(String!, for: ABPerson!, byExtendingSelection: Bool)

Selects a value or a set of values in a multivalue property.

func select(ABRecord!, byExtendingSelection: Bool)

Selects a record or a set of records in the record list.


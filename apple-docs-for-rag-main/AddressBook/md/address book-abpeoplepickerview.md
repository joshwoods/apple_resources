

- Address Book
-  ABPeoplePickerView 

Class

# ABPeoplePickerView

An object you use to customize the behavior of people-picker views in an app’s user interface.

macOS 10.3+

``` source
@MainActor
class ABPeoplePickerView
```

## Topics

### Working with Properties in the Record List

func addProperty(String!)

Adds a property to the group of properties whose values are shown in the record list.

func columnTitle(forProperty: String!) -> String!

Returns the title of a custom property.

var displayedProperty: String!

The property currently displayed in the record list.

func properties() -> [Any]!

Returns an array of the properties whose values are shown in the record list.

func removeProperty(String!)

Removes a property from the group of properties whose values are shown in the record list.

func setColumnTitle(String!, forProperty: String!)

Sets the title displayed in the people picker for a property.

### Specifying Selection Behavior

var valueSelectionBehavior: ABPeoplePickerSelectionBehavior

The current selection behavior.

struct ABPeoplePickerSelectionBehavior

Constants indicating the possible value selection behaviors.

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

func selectedIdentifiers(for: ABPerson!) -> [Any]!

Returns the identifiers of the selected values in a multivalue property.

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

### Specifying the Accessory View

var accessoryView: NSView!

The view that is placed to the left of the search field.

### Managing Actions

func clearSearchField(Any!)

Clears the search field and resets the list of displayed records.

func editInAddressBook(Any!)

Launches Address Book to edit the item selected in the people picker.

var groupDoubleAction: Selector!

The action to be invoked when a group is double-clicked.

var nameDoubleAction: Selector!

The action to be invoked when a name is double-clicked.

func selectInAddressBook(Any!)

Launches Address Book and selects the item selected in the people picker.

var target: AnyObject!

The target for double-click actions.

### Managing Persistent User Settings

var autosaveName: String!

The name under which the column positions and the filter selection are saved.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification

## See Also

### Pickers

class ABPersonView

An object that provides a view for displaying and editing contacts.


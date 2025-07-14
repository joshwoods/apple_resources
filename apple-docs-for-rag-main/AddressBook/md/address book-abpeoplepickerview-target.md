

- Address Book
- ABPeoplePickerView
-  target 

Instance Property

# target

The target for double-click actions.

macOS 10.3+

``` source
@MainActor
unowned(unsafe) var target: AnyObject! { get set }
```

## Discussion

The target is the object on which the action specified by groupDoubleAction and nameDoubleAction is invoked.

## See Also

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


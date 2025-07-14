

- Address Book
- ABPeoplePickerView
-  editInAddressBook(\_:) 

Instance Method

# editInAddressBook(\_:)

Launches Address Book to edit the item selected in the people picker.

macOS

``` source
@MainActor
func editInAddressBook(_ sender: Any!)
```

## Parameters 

`sender`  

The object sending this message.

## See Also

### Managing Actions

func clearSearchField(Any!)

Clears the search field and resets the list of displayed records.

var groupDoubleAction: Selector!

The action to be invoked when a group is double-clicked.

var nameDoubleAction: Selector!

The action to be invoked when a name is double-clicked.

func selectInAddressBook(Any!)

Launches Address Book and selects the item selected in the people picker.

var target: AnyObject!

The target for double-click actions.


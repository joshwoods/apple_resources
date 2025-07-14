

- Foundation
- NSNotification
- NSNotification.Name
-  abDatabaseChanged 

Type Property

# abDatabaseChanged

Posted when this process has changed the Address Book database.

macOS 10.0+

``` source
static let abDatabaseChanged: NSNotification.Name
```

## Discussion

Depending on the operation performed on the address book, one or more of the following keys may be included in the user-info dictionary: `kABInsertedRecords`, `kABUpdatedRecords`, and `kABDeletedRecords`. The values for each of the keys are the unique IDs of the records that were inserted, updated, or deleted, respectively. If the values for all the keys are `nil`, every record has changes. For example, this happens when the Address Book database is restored from a backup copy.

Note

The system posts this notification on the main actor.

## See Also

### AddressBook

static let abDatabaseChangedExternally: NSNotification.Name

Posted when a process other than the current one has changed the Address Book database.

static let ABPeoplePickerDisplayedPropertyDidChange: NSNotification.Name

Posted when the displayed property in the record list is changed.

static let ABPeoplePickerGroupSelectionDidChange: NSNotification.Name

Posted when the selection in the group list is changed.

static let ABPeoplePickerNameSelectionDidChange: NSNotification.Name

Posted when the selection in the name list is changed.

static let ABPeoplePickerValueSelectionDidChange: NSNotification.Name

Posted when the selection in a multivalue property is changed.


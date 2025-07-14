

- Address Book
-  AddressBook Functions 

API Collection

# AddressBook Functions

Find the C functions and function-like macros you use to manipulate Address Book data.

## Topics

### Address Book

func ABGetSharedAddressBook() -> Unmanaged&lt;ABAddressBookRef>!

Returns the unique shared ABAddressBook object.

func ABCopyDefaultCountryCode(ABAddressBookRef!) -> Unmanaged&lt;CFString>!

Returns the default country code for records with unspecified country codes.

func ABHasUnsavedChanges(ABAddressBookRef!) -> Bool

Returns whether if there are unsaved changes in the address book.

func ABSave(ABAddressBookRef!) -> Bool

Saves all the changes made since the last save.

### People

func ABCopyArrayOfAllPeople(ABAddressBookRef!) -> Unmanaged&lt;CFArray>!

Returns an array of all the people in the Address Book database.

func ABGetMe(ABAddressBookRef!) -> Unmanaged&lt;ABPersonRef>!

Returns the ABPerson object for the logged-in user.

func ABPersonCopyImageData(ABRecord!) -> Unmanaged&lt;CFData>!

Returns data that contains a picture of a person.

Deprecated

func ABPersonCopyParentGroups(ABPersonRef!) -> Unmanaged&lt;CFArray>!

Returns an array of groups that a person belongs to.

func ABPersonCopyVCardRepresentation(ABPersonRef!) -> Unmanaged&lt;CFData>!

Returns the vCard representation of the person as a data object in vCard format.

func ABPersonCreate() -> Unmanaged&lt;ABRecord>!

Returns a newly created person object.

Deprecated

func ABPersonCreateSearchElement(CFString!, CFString!, CFString!, CFTypeRef!, ABSearchComparison) -> Unmanaged&lt;ABSearchElementRef>!

Returns a search element object that specifies a query for records of this type.

func ABPersonCreateWithVCardRepresentation(CFData!) -> Unmanaged&lt;ABPersonRef>!

Returns a new ABPerson object initialized with the given data in vCard format.

func ABPersonSetImageData(ABRecord!, CFData!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the image for this person to the given data.

Deprecated

func ABSetMe(ABAddressBookRef!, ABPersonRef!)

Sets the record that represents the logged-in user.

### Groups

func ABCopyArrayOfAllGroups(ABAddressBookRef!) -> Unmanaged&lt;CFArray>!

Returns an array of all the groups in the Address Book database.

func ABGroupAddGroup(ABGroupRef!, ABGroupRef!) -> Bool

Adds a subgroup to another group.

func ABGroupAddMember(ABRecord!, ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Adds a person to a group.

Deprecated

func ABGroupCopyArrayOfAllMembers(ABRecord!) -> Unmanaged&lt;CFArray>!

Returns an array of persons in a group.

Deprecated

func ABGroupCopyArrayOfAllSubgroups(ABGroupRef!) -> Unmanaged&lt;CFArray>!

Returns an array containing a group’s subgroups.

func ABGroupCopyDistributionIdentifier(ABGroupRef!, ABPersonRef!, CFString!) -> Unmanaged&lt;CFString>!

Returns the distribution identifier for the given propertyand person.

func ABGroupCopyParentGroups(ABGroupRef!) -> Unmanaged&lt;CFArray>!

Returns an array containing a group’s parents—thegroups that a group belongs to.

func ABGroupCreate() -> Unmanaged&lt;ABRecord>!

Returns a new ABGroup object.

Deprecated

func ABGroupCreateSearchElement(CFString!, CFString!, CFString!, CFTypeRef!, ABSearchComparison) -> Unmanaged&lt;ABSearchElementRef>!

Creates an ABSearchElement object that specifies a queryfor ABGroup records.

func ABGroupRemoveGroup(ABGroupRef!, ABGroupRef!) -> Bool

Removes a subgroup from a group.

func ABGroupRemoveMember(ABRecord!, ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a person from a group.

Deprecated

func ABGroupSetDistributionIdentifier(ABGroupRef!, ABPersonRef!, CFString!, CFString!) -> Bool

Assigning a specific distribution identifier for a person’smulti-value list property so that the group can be used as a distributionlist (mailing list, in the case of an email property).

### Multi Values

func ABMultiValueAdd(ABMutableMultiValueRef!, CFTypeRef!, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Bool

Adds a value and its label to a multi-value list.

func ABMultiValueCopyIdentifierAtIndex(ABMultiValueRef!, CFIndex) -> Unmanaged&lt;CFString>!

Returns the identifier at the given index.

func ABMultiValueCopyLabelAtIndex(ABMultiValue!, CFIndex) -> Unmanaged&lt;CFString>!

Returns the label for the given index.

Deprecated

func ABMultiValueCopyPrimaryIdentifier(ABMultiValueRef!) -> Unmanaged&lt;CFString>!

Returns the identifier for the primary value.

func ABMultiValueCopyValueAtIndex(ABMultiValue!, CFIndex) -> Unmanaged&lt;CFTypeRef>!

Returns the value for the given index.

Deprecated

func ABMultiValueCount(ABMultiValueRef!) -> CFIndex

Returns the number of entries in a multi-value list.

func ABMultiValueCreate() -> Unmanaged&lt;ABMultiValueRef>!

Returns a new ABMultiValue object.

func ABMultiValueCreateCopy(ABMultiValueRef!) -> Unmanaged&lt;ABMultiValueRef>!

Returns a copy of a multi-value object.

func ABMultiValueCreateMutable(ABPropertyType) -> Unmanaged&lt;ABMutableMultiValue>!

Returns a newly created mutable multi-value list object.

Deprecated

func ABMultiValueCreateMutableCopy(ABMultiValue!) -> Unmanaged&lt;ABMutableMultiValue>!

Returns a mutable copy of a multi-value object.

Deprecated

func ABMultiValueIndexForIdentifier(ABMultiValueRef!, CFString!) -> CFIndex

Returns the index for the given identifier.

func ABMultiValueInsert(ABMutableMultiValueRef!, CFTypeRef!, CFString!, CFIndex, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Bool

Inserts a value and its label at the given index in amulti-value list.

func ABMultiValuePropertyType(ABMultiValueRef!) -> ABPropertyType

Returns the type for the values in a multi-value list.

func ABMultiValueRemove(ABMutableMultiValueRef!, CFIndex) -> Bool

Removes the value and label at the given index.

func ABMultiValueReplaceLabel(ABMutableMultiValueRef!, CFString!, CFIndex) -> Bool

Replaces the label at the given index.

func ABMultiValueReplaceValue(ABMutableMultiValueRef!, CFTypeRef!, CFIndex) -> Bool

Replaces the value at the given index.

func ABMultiValueSetPrimaryIdentifier(ABMutableMultiValueRef!, CFString!) -> Bool

Sets the primary value to be the value for the given identifier.

### Images

func ABBeginLoadingImageDataForClient(ABPersonRef!, ABImageClientCallback!, UnsafeMutableRawPointer!) -> CFIndex

Starts an asynchronous fetch for image data in all locations, and returns a non-zero tag for tracking.

func ABCancelLoadingImageDataForTag(CFIndex)

Cancels an asynchronous fetch of an image for the given tag.

### Search Elements

func ABCopyArrayOfMatchingRecords(ABAddressBookRef!, ABSearchElementRef!) -> Unmanaged&lt;CFArray>!

Returns an array of records that match the given search element, or an empty array if no records match the search element.

func ABSearchElementCreateWithConjunction(ABSearchConjunction, CFArray!) -> Unmanaged&lt;ABSearchElementRef>!

Returns a compound search element created by combiningthe search elements in an array with the given conjunction.

func ABSearchElementMatchesRecord(ABSearchElementRef!, ABRecordRef!) -> Bool

Tests whether or not a record matches a search element.

### Properties

func ABAddPropertiesAndTypes(ABAddressBookRef!, CFString!, CFDictionary!) -> CFIndex

Adds the given properties to all the records of the specified type in the Address Book database, and returns the number of properties successfully added.

func ABCopyArrayOfPropertiesForRecordType(ABAddressBookRef!, CFString!) -> Unmanaged&lt;CFArray>!

Returns an array containing the names of all the properties for the specified record type.

func ABCopyLocalizedPropertyOrLabel(CFString!) -> Unmanaged&lt;CFString>!

Returns the localized version of a built in property,label, or key.

func ABLocalizedPropertyOrLabel(String!) -> String!

Returns the localized version of a built in property, label, or key.

func ABRemoveProperties(ABAddressBookRef!, CFString!, CFArray!) -> CFIndex

Removes the given properties from all the records of this type in the Address Book database, and returns the number of properties successfully removed.

func ABTypeOfProperty(ABAddressBookRef!, CFString!, CFString!) -> ABPropertyType

Returns the type of a given property for a given record.

### Records

func ABAddRecord(ABAddressBookRef!, ABRecordRef!) -> Bool

Adds a record of the specified type to the Address Book database.

func ABCopyRecordForUniqueId(ABAddressBookRef!, CFString!) -> Unmanaged&lt;ABRecordRef>!

Returns the record that matches the given unique ID.

func ABCopyRecordTypeFromUniqueId(ABAddressBookRef!, CFString!) -> Unmanaged&lt;CFString>!

Returns the type name of the record that matches a given unique ID.

func ABCreateFormattedAddressFromDictionary(ABAddressBookRef!, CFDictionary!) -> Unmanaged&lt;CFString>!

Returns a string containing the formatted address.

func ABRecordCopyRecordType(ABRecordRef!) -> Unmanaged&lt;CFString>!

Returns the type of the given record.

func ABRecordCopyUniqueId(ABRecordRef!) -> Unmanaged&lt;CFString>!

Returns the unique ID of the receiver.

func ABRecordCopyValue(ABRecord!, ABPropertyID) -> Unmanaged&lt;CFTypeRef>!

Returns the value of the given property.

Deprecated

func ABRecordCreateCopy(ABRecordRef!) -> Unmanaged&lt;ABRecordRef>!

Returns a copy of the given record.

func ABRecordIsReadOnly(ABRecordRef!) -> Bool

Returns whether or not the record is read-only.

func ABRecordRemoveValue(ABRecord!, ABPropertyID, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes the value of the given property.

Deprecated

func ABRecordSetValue(ABRecord!, ABPropertyID, CFTypeRef!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Sets the value of a given property for a record.

Deprecated

func ABRemoveRecord(ABAddressBookRef!, ABRecordRef!) -> Bool

Removes the specified record from the Address Book database.

### Deprecated

func ABAddressBookAddRecord(ABAddressBook!, ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Adds a record to an address book.

Deprecated

func ABAddressBookCopyArrayOfAllGroups(ABAddressBook!) -> Unmanaged&lt;CFArray>!

Returns an array with all the groups in an address book.

Deprecated

func ABAddressBookCopyArrayOfAllGroupsInSource(ABAddressBook!, ABRecord!) -> Unmanaged&lt;CFArray>!

Returns an array of all groups from a particular source.

Deprecated

func ABAddressBookCopyArrayOfAllPeople(ABAddressBook!) -> Unmanaged&lt;CFArray>!

Returns all the person records in an address book.

Deprecated

func ABAddressBookCopyArrayOfAllPeopleInSource(ABAddressBook!, ABRecord!) -> Unmanaged&lt;CFArray>!

Returns an array of all person records from a particular source.

Deprecated

func ABAddressBookCopyArrayOfAllPeopleInSourceWithSortOrdering(ABAddressBook!, ABRecord!, ABPersonSortOrdering) -> Unmanaged&lt;CFArray>!

Returns an array of all person records in the address book, sorted with the specified order.

Deprecated

func ABAddressBookCopyArrayOfAllSources(ABAddressBook!) -> Unmanaged&lt;CFArray>!

Returns an array of all sources in the address book.

Deprecated

func ABAddressBookCopyDefaultSource(ABAddressBook!) -> Unmanaged&lt;ABRecord>!

Returns the default source.

Deprecated

func ABAddressBookCopyLocalizedLabel(CFString!) -> Unmanaged&lt;CFString>!

Returns a localized version of a record-property label.

Deprecated

func ABAddressBookCopyPeopleWithName(ABAddressBook!, CFString!) -> Unmanaged&lt;CFArray>!

Performs a prefix search on the composite names of people in an address book and returns an array of persons that match the search criteria.

Deprecated

func ABAddressBookCreate() -> Unmanaged&lt;ABAddressBook>!

Creates a new address book object with data from the Address Book database.

Deprecated

func ABAddressBookCreateWithOptions(CFDictionary!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;ABAddressBook>!

Creates a new address book object with data from the Address Book database.

Deprecated

func ABAddressBookGetAuthorizationStatus() -> ABAuthorizationStatus

Returns the authorization status of your app for accessing address book data.

Deprecated

func ABAddressBookGetGroupCount(ABAddressBook!) -> CFIndex

Returns the number of groups in an address book.

Deprecated

func ABAddressBookGetGroupWithRecordID(ABAddressBook!, ABRecordID) -> Unmanaged&lt;ABRecord>!

Returns the group with a given record ID.

Deprecated

func ABAddressBookGetPersonCount(ABAddressBook!) -> CFIndex

Returns the number of person records in an address book.

Deprecated

func ABAddressBookGetPersonWithRecordID(ABAddressBook!, ABRecordID) -> Unmanaged&lt;ABRecord>!

Returns the person record with a given record ID.

Deprecated

func ABAddressBookGetSourceWithRecordID(ABAddressBook!, ABRecordID) -> Unmanaged&lt;ABRecord>!

Returns the source record with the given record ID.

Deprecated

func ABAddressBookHasUnsavedChanges(ABAddressBook!) -> Bool

Indicates whether an address book has changes that have not been saved to the Address Book database.

Deprecated

func ABAddressBookRegisterExternalChangeCallback(ABAddressBook!, ABExternalChangeCallback!, UnsafeMutableRawPointer!)

Registers a callback to receive notifications when the Address Book database is modified.

Deprecated

func ABAddressBookRemoveRecord(ABAddressBook!, ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a record from an address book.

Deprecated

func ABAddressBookRequestAccessWithCompletion(ABAddressBook!, ABAddressBookRequestAccessCompletionHandler!)

Requests access to address book data from the user.

Deprecated

func ABAddressBookRevert(ABAddressBook!)

Discards unsaved changes in an address book.

Deprecated

func ABAddressBookSave(ABAddressBook!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Saves any unsaved changes to the Address Book database.

Deprecated

func ABAddressBookUnregisterExternalChangeCallback(ABAddressBook!, ABExternalChangeCallback!, UnsafeMutableRawPointer!)

Unregisters a callback.

Deprecated

func ABGroupCopyArrayOfAllMembersWithSortOrdering(ABRecord!, ABPersonSortOrdering) -> Unmanaged&lt;CFArray>!

Returns the records in a group, using a sort ordering.

Deprecated

func ABGroupCopySource(ABRecord!) -> Unmanaged&lt;ABRecord>!

Returns the source that the group is from.

Deprecated

func ABGroupCreateInSource(ABRecord!) -> Unmanaged&lt;ABRecord>!

Creates a group in a particular source.

Deprecated

func ABMultiValueAddValueAndLabel(ABMutableMultiValue!, CFTypeRef!, CFString!, UnsafeMutablePointer&lt;ABMultiValueIdentifier>!) -> Bool

Adds a value and its corresponding label to a multivalue property.

Deprecated

func ABMultiValueCopyArrayOfAllValues(ABMultiValue!) -> Unmanaged&lt;CFArray>!

Returns an array with the values in a multivalue property.

Deprecated

func ABMultiValueGetCount(ABMultiValue!) -> CFIndex

Returns the number of values in a multivalue property.

Deprecated

func ABMultiValueGetFirstIndexOfValue(ABMultiValue!, CFTypeRef!) -> CFIndex

Returns the first location of a value in a multivalue property.

Deprecated

func ABMultiValueGetIdentifierAtIndex(ABMultiValue!, CFIndex) -> ABMultiValueIdentifier

Returns the identifier of a value in a multivalue property.

Deprecated

func ABMultiValueGetIndexForIdentifier(ABMultiValue!, ABMultiValueIdentifier) -> CFIndex

Returns the location (within a multivalue property) of a value with a given identifier.

Deprecated

func ABMultiValueGetPropertyType(ABMultiValue!) -> ABPropertyType

Returns the type of the values contained in a multivalue property.

Deprecated

func ABMultiValueInsertValueAndLabelAtIndex(ABMutableMultiValue!, CFTypeRef!, CFString!, CFIndex, UnsafeMutablePointer&lt;ABMultiValueIdentifier>!) -> Bool

Inserts a value and a label into a multivalue property.

Deprecated

func ABMultiValueRemoveValueAndLabelAtIndex(ABMutableMultiValue!, CFIndex) -> Bool

Removes a value from a multivalue property.

Deprecated

func ABMultiValueReplaceLabelAtIndex(ABMutableMultiValue!, CFString!, CFIndex) -> Bool

Replaces a label in a multivalue property with another label.

Deprecated

func ABMultiValueReplaceValueAtIndex(ABMutableMultiValue!, CFTypeRef!, CFIndex) -> Bool

Replaces a value in a multivalue property with another value.

Deprecated

func ABPersonComparePeopleByName(ABRecord!, ABRecord!, ABPersonSortOrdering) -> CFComparisonResult

Indicates how two person records get sorted.

Deprecated

func ABPersonCopyArrayOfAllLinkedPeople(ABRecord!) -> Unmanaged&lt;CFArray>!

Returns an array of all person records in the address book database that are linked to the given person record.

Deprecated

func ABPersonCopyCompositeNameDelimiterForRecord(ABRecord!) -> Unmanaged&lt;CFString>!

Returns the delimiter to use between name components.

Deprecated

func ABPersonCopyImageDataWithFormat(ABRecord!, ABPersonImageFormat) -> Unmanaged&lt;CFData>!

Returns the picture for a person record in the given format.

Deprecated

func ABPersonCopyLocalizedPropertyName(ABPropertyID) -> Unmanaged&lt;CFString>!

Returns the localized name of a person property

Deprecated

func ABPersonCopySource(ABRecord!) -> Unmanaged&lt;ABRecord>!

Returns the source that the person record is from.

Deprecated

func ABPersonCreateInSource(ABRecord!) -> Unmanaged&lt;ABRecord>!

Creates a new person record in a particular source.

Deprecated

func ABPersonCreatePeopleInSourceWithVCardRepresentation(ABRecord!, CFData!) -> Unmanaged&lt;CFArray>!

Creates person records from the given vCard representation.

Deprecated

func ABPersonCreateVCardRepresentationWithPeople(CFArray!) -> Unmanaged&lt;CFData>!

Returns the vCard representation of the given person records.

Deprecated

func ABPersonGetCompositeNameFormat() -> ABPersonCompositeNameFormat

Returns the person-name display format.

Deprecated

func ABPersonGetCompositeNameFormatForRecord(ABRecord!) -> ABPersonCompositeNameFormat

Returns the person-name display format to use for the given record.

Deprecated

func ABPersonGetSortOrdering() -> ABPersonSortOrdering

Returns the user’s sort-ordering preference for lists of persons.

Deprecated

func ABPersonGetTypeOfProperty(ABPropertyID) -> ABPropertyType

Returns the type of a person property.

Deprecated

func ABPersonHasImageData(ABRecord!) -> Bool

Indicates whether a person has a picture.

Deprecated

func ABPersonRemoveImageData(ABRecord!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Bool

Removes a person’s picture.

Deprecated

func ABRecordCopyCompositeName(ABRecord!) -> Unmanaged&lt;CFString>!

Returns an appropriate, human-friendly name for the record.

Deprecated

func ABRecordGetRecordID(ABRecord!) -> ABRecordID

Returns the unique ID of a record.

Deprecated

func ABRecordGetRecordType(ABRecord!) -> ABRecordType

Returns the type of a record.

Deprecated

## See Also

### C Interfaces

C Types

Identify the C types that correspond to Address Book objects.

Address Book Constants

Get the constants you use to specify Address Book information.

AddressBook Enumerations

Get the enumerations you use to specify Address Book information.

AddressBook Data Types

Get the data types you use to specify Address Book information.


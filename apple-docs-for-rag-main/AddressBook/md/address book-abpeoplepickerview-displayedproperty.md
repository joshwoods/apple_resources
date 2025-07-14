

- Address Book
- ABPeoplePickerView
-  displayedProperty 

Instance Property

# displayedProperty

The property currently displayed in the record list.

macOS 10.3+

``` source
@MainActor
var displayedProperty: String! { get set }
```

## See Also

### Working with Properties in the Record List

func addProperty(String!)

Adds a property to the group of properties whose values are shown in the record list.

func columnTitle(forProperty: String!) -> String!

Returns the title of a custom property.

func properties() -> [Any]!

Returns an array of the properties whose values are shown in the record list.

func removeProperty(String!)

Removes a property from the group of properties whose values are shown in the record list.

func setColumnTitle(String!, forProperty: String!)

Sets the title displayed in the people picker for a property.


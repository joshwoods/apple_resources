

- Address Book
- ABPeoplePickerView
-  columnTitle(forProperty:) 

Instance Method

# columnTitle(forProperty:)

Returns the title of a custom property.

macOS 10.3+

``` source
@MainActor
func columnTitle(forProperty property: String!) -> String!
```

## Parameters 

`property`  

The property whose title will be returned.

## Return Value

The title of the custom property.

## See Also

### Working with Properties in the Record List

func addProperty(String!)

Adds a property to the group of properties whose values are shown in the record list.

var displayedProperty: String!

The property currently displayed in the record list.

func properties() -> [Any]!

Returns an array of the properties whose values are shown in the record list.

func removeProperty(String!)

Removes a property from the group of properties whose values are shown in the record list.

func setColumnTitle(String!, forProperty: String!)

Sets the title displayed in the people picker for a property.


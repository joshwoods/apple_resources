

- Address Book
- ABPeoplePickerView
-  addProperty(\_:) 

Instance Method

# addProperty(\_:)

Adds a property to the group of properties whose values are shown in the record list.

macOS 10.3+

``` source
@MainActor
func addProperty(_ property: String!)
```

## Parameters 

`property`  

The property to add.

## Discussion

For additional information about properties see Constants.

## See Also

### Working with Properties in the Record List

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


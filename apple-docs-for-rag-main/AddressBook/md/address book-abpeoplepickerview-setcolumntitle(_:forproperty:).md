

- Address Book
- ABPeoplePickerView
-  setColumnTitle(\_:forProperty:) 

Instance Method

# setColumnTitle(\_:forProperty:)

Sets the title displayed in the people picker for a property.

macOS 10.3+

``` source
@MainActor
func setColumnTitle(
    _ title: String!,
    forProperty property: String!
)
```

## Parameters 

`title`  

The title to be set.

`property`  

The property being titled.

## See Also

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


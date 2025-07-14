

- TVMLKit JS
- Keyboard
-  suggestions 

Instance Property

# suggestions

Search parameters to offer as shortcuts.

tvOS 14.0+

``` source
attribute Array suggestions;
```

## Discussion

Provide search suggestions to help the user complete their query quickly. Update the suggestions as the user types. This property is only available if the Keyboard is associated with a searchField.

Each suggestion in this array should have the following properties:

`text`  
A label for the suggestion, usually the search term the suggestion represents.

`badge`  
The name of an image for display alongside the suggestion’s text. This property is optional.

`searchTerm`  
A string containing search criteria. This property is optional.

## See Also

### Providing and Handling Search Suggestions

onSuggestionSelected

A function the system calls when the user selects a suggestion on a search field.


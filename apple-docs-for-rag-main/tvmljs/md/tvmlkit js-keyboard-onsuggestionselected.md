

- TVMLKit JS
- Keyboard
-  onSuggestionSelected 

Instance Property

# onSuggestionSelected

A function the system calls when the user selects a suggestion on a search field.

tvOS 14.0+

``` source
attribute function onSuggestionSelected;
```

## Discussion

Provide a callback function for the `onSuggestionSelected` attribute to respond to the user selecting one of a `searchField`’s suggestions. This value of this attribute must be a function; for example, k`eyboard.onSuggestionSelected = function (searchTerm) {}`.

## See Also

### Providing and Handling Search Suggestions

suggestions

Search parameters to offer as shortcuts.




- TVMLKit JS
-  Keyboard 

Class

# Keyboard

An object used to retrieve user input from search fields and text fields.

tvOS 9.0+

``` source
interface Keyboard
```

## Overview

Use the `getFeature` function with the feature name `Keyboard` to retrieve an instance of this class from the `searchField` and `textField` elements, as in, for example, `getFeature('Keyboard')`.

## Topics

### Setting and Retrieving Text

text

The text inside a search or text field.

onTextChange

A function the system calls when the text in a search or text field changes.

### Providing and Handling Search Suggestions

suggestions

Search parameters to offer as shortcuts.

onSuggestionSelected

A function the system calls when the user selects a suggestion on a search field.

## See Also

### Element Access

MenuBarDocument

An object used for setting and retrieving documents associated with a menu item.


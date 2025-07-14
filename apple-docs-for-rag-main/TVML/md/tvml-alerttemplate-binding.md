

- TVML
- alertTemplate
-  binding 

Article

# binding

Associates information in a data item with an element.

## Overview

Use the `binding` attribute to associate the property path in a data item with an element.

Note

For more information on binding, see Manipulating the Document Object Model (DOM) in the TVML Programming Guide.

### Values for binding

`@:{value}`  
The attribute tag and value. For example, `` adds the `src` attribute with the URL found in the associated data item.

`items:{property path}`  
The item associated with the specified property path.

`textContent:{property path}`  
The text associated with the specified property path.

### Elements that Use binding

The `binding` attribute can be used with any element.

## See Also

### Valid TVML Attributes

autoHighlight

Specifies that the element should initially be in focus.

layoutDirection

Specifies the direction in which text is displayed.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.


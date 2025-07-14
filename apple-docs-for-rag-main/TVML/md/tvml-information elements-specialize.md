

- TVML
- Information Elements
-  specialize 

# specialize

Implements queries used for data binding.

## Overview

The `specialize` element is used to modify an existing element based on a data query. Combine the query with parameters contained in your JSON data to determine how to modify an existing element. Here’s an example that changes the text for a button if the user has started watching a media item, but hasn’t finished it.

```

        Resume

```

### Subelements of specialize

The `specialize` element can contain any element.

### Elements that Use specialize

- rules

## Topics

### Valid TVML Attributes

binding

Associates information in a data item with an element.

prototype

Associates a data item type with an element.

theme

Sets the color scheme for an element.

## See Also

### Binding Elements

prototypes

Defines a group of elements that can be reused through binding.

rules

Contains the elements used in data binding and media queries.


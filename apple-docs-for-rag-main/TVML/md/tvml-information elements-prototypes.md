

- TVML
- Information Elements
-  prototypes 

# prototypes

Defines a group of elements that can be reused through binding.

## Overview

The `prototypes` element is used to bind data item types, simplifying the template layout. A single binding definition provides the ability to display any number of data items. For more information on data binding, see TVML Programming Guide. Here’s an example that uses the `prototypes` element to display an undefined number of `lockup` elements.

```

```

### Subelements of prototypes

`prototypes` can contain any element that can be contained by a `section` element. The child elements must implement the `prototype` attribute to bind the correct data items.

### Elements that Use prototypes

`The prototypes` element can be a used by any element.

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

rules

Contains the elements used in data binding and media queries.

specialize

Implements queries used for data binding.


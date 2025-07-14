

- TVML
- Data Binding Queries
-  {property-path} 

Article

# {property-path}

Compares a value from a JSON file to a specified value to find out if they are equal.

## Overview

The `{property-path}` query is used with data binding to determine whether one value is equal to another. Bind a value from your JSON file to a variable associated with the query. If the `property-path` is equal to the designated value, the element is processed.

For example, you want to change the title of a movie if the user has never watched it. Add a `specialize` element that contains a `{property-path}` query. If the `timesPlayed` variable is equal to 0, color the title white.

```

```


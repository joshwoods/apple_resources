

- Apple Search Ads
-  Condition 

Object

# Condition

The list of condition objects that allow users to filter a list of records.

Search Ads 2.0+

``` source
object Condition
```

## Properties

`field`

`string`

The name of a field.

`ignoreCase`

`boolean`

`operator`

`string`

The operator values compare attributes to a list of specified values.

BETWEEN  
The attribute matches the values within a specified range. The values can be numbers, text, or dates.

CONTAINS  
The attribute matches the value in the specified list.

CONTAINS_ALL  
The attribute has all of the values in the specified list.

The attribute must be a collection type.

CONTAINS_ANY  
The attribute contains any of the values in the specified list.

The attribute must be a collection type.

ENDSWITH  
The attribute matches the suffix of a string.

EQUALS  
The attribute contains exact values.

GREATER_THAN  
The value is greater than the specified value.

You can use this attribute with time parameters.

IN  
The attribute matches any value in a list of specified values.

LESS_THAN  
The value is less than the specified value.

You can use this attribute with time parameters.

STARTSWITH  
The attribute matches the prefix of a string.

Possible Values: `BETWEEN, CONTAINS, CONTAINS_ALL, CONTAINS_ANY, ENDSWITH, EQUALS, GREATER_THAN, IN, LESS_THAN, LIKE, STARTSWITH`

`values`

`[string]`

A list of matching values.

## Mentioned in 

Apple Search Ads Campaign Management API 5

## Discussion

The `Condition` object functionality is similar to the `WHERE` clause in SQL.

## See Also

### API Usability

object PageDetail

The number of items that return in the page.

object Pagination

The procedure to refine returned results using limit and offset parameters.

object Selector

The selector objects available to filter returned data.

object Sorting

The order of grouped results.


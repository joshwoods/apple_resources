

- Apple Search Ads
-  Selector 

Object

# Selector

The selector objects available to filter returned data.

Search Ads 2.0+

``` source
object Selector
```

## Properties

`conditions`

`[`Condition`]`

A list of condition objects that allow users to filter a list of records.

`fields`

`[string]`

A list of field names to return within each record.

`orderBy`

`[`Sorting`]`

A list of field names and grouping to sort the records by `ASCENDING` or `DESCENDING`.

`pagination`

Pagination

A defined range and limit of the number of returned records.

## Discussion

Selector objects define what data the API returns when fetching resources. You use Selector objects with find calls and reporting endpoints.

| **Functionality** | **Description** |
|----|----|
| Filtering | Specifies the criteria to filter the resources that return. |
| Sorting | Specifies the criteria to order the resources that return. |
| Paginating | Specifies the page segment of resources that return. |

The following is an example of using selectors to filter returned records:

```
POST https://api.searchads.apple.com/api/v5/campaigns/find

{  
  "fields": [
    "id",
    "name",
    "adamId",
    "budgetAmount",
    "dailyBudgetAmount",
    "status",
    "servingStatus"
  ],
  "conditions": [
    {
      "field": "servingStatus",
      "operator": "IN",
      "values": [
        "NOT_RUNNING"
      ]
    }
  ],
  "orderBy": [
    {
      "field": "id",
      "sortOrder": "DESCENDING"
    }
  ],
  "pagination": {
    "offset": 0,
    "limit": 10
  }
}

```

You can also use Selector objects to find archived or soft-deleted campaigns. By default, API fetch calls don’t return deleted resources, with the exception of GET by `a` resource `Id`. To retrieve deleted resources, you must explicitly request the call using the selector Condition.

The following example returns both deleted and undeleted resources:

```
{
  "fields": null,
  "conditions": [
    {
      "field": "deleted",
      "operator": "IN",
      "values": [
        true,
        false
      ]
    }
  ],
  "orderBy": [
    {
      "field": "name",
      "sortOrder": "ASCENDING"
    }
  ],
  "pagination": {
    "offset": 0,
    "limit": 100
  }
}

```

## See Also

### API Usability

object Condition

The list of condition objects that allow users to filter a list of records.

object PageDetail

The number of items that return in the page.

object Pagination

The procedure to refine returned results using limit and offset parameters.

object Sorting

The order of grouped results.


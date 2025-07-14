

- Apple Search Ads
-  BudgetOrderInfo 

Object

# BudgetOrderInfo

The parent object response to a request for budget order details.

Search Ads 2.0+

``` source
object BudgetOrderInfo
```

## Properties

`bo`

BudgetOrder

The details of the budget order.

`orgIds`

`[int64]`

The identifier of the organization that owns the campaign. Currently, only one `orgId` is supported.

## See Also

### Budget Order Request and Response Objects

object BudgetOrder

The response to requests for budget order details.

object BudgetOrderCreate

The parent object response to a request to create a budget order.

object BudgetOrderUpdate

The parent object response to a request to update a budget order.

object BudgetOrderInfoResponse

A container for the budget order response body.

object BudgetOrderInfoListResponse

The response details to budget order requests.

object LOCInvoiceDetails

The response to a request to fetch details for a monthly invoicing payment model.

object Money

The response to requests for budget amounts in campaigns.


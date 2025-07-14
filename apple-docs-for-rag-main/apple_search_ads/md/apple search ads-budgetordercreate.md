

- Apple Search Ads
-  BudgetOrderCreate 

Object

# BudgetOrderCreate

The parent object response to a request to create a budget order.

Search Ads 4.11+

``` source
object BudgetOrderCreate
```

## Properties

`bo`

BudgetOrderCreate.Bo

Contains the details of the budget order.

`orgIds`

`[int64]`

The identifier of the organization that owns the campaign. Currently, only one `orgId` is supported.

## Topics

### Objects

object BudgetOrderCreate.Bo

The response to a request to create a budget order.

## See Also

### Budget Order Request and Response Objects

object BudgetOrder

The response to requests for budget order details.

object BudgetOrderInfo

The parent object response to a request for budget order details.

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


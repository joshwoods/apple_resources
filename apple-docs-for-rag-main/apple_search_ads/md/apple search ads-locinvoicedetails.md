

- Apple Search Ads
-  LOCInvoiceDetails 

Object

# LOCInvoiceDetails

The response to a request to fetch details for a monthly invoicing payment model.

Search Ads 2.0+

``` source
object LOCInvoiceDetails
```

## Properties

`billingContactEmail`

`string`

A valid email address for the LOC billing contact.

`buyerEmail`

`string`

A valid email address for the LOC buyer.

`buyerName`

`string`

A valid LOC buyer name.

`clientName`

`string`

An advertiser or product. Required for agency-type accounts.

`orderNumber`

`string`

A purchase order number. Required for agency-type accounts.

## See Also

### Budget Order Request and Response Objects

object BudgetOrder

The response to requests for budget order details.

object BudgetOrderInfo

The parent object response to a request for budget order details.

object BudgetOrderCreate

The parent object response to a request to create a budget order.

object BudgetOrderUpdate

The parent object response to a request to update a budget order.

object BudgetOrderInfoResponse

A container for the budget order response body.

object BudgetOrderInfoListResponse

The response details to budget order requests.

object Money

The response to requests for budget amounts in campaigns.


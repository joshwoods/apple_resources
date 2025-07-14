

- Apple Search Ads
-  Money 

Object

# Money

The response to requests for budget amounts in campaigns.

Search Ads 2.0+

``` source
object Money
```

## Properties

`amount`

`string`

The monetary value in the specified currency. The API uses `amount` whenever a currency value is necessary. The string can contain up to two decimal digits.

`currency`

`string`

The organization’s default currency that is set up in the Apple Search Ads UI.

Possible Values: `AUD, CAD, EUR, GBP, JPY, MXN, NZD, RUB, USD`

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

object LOCInvoiceDetails

The response to a request to fetch details for a monthly invoicing payment model.


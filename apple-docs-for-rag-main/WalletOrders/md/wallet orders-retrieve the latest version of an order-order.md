

- Wallet Orders
-  Retrieve the latest version of an order 

Web Service Endpoint

# Retrieve the latest version of an order

Retrieves the latest signed and compressed version of an order.

iOS 16.0+iPadOS 16.0+macOS 13.0+

## URL

``` source
GET https://your-web-service.com/v1/orders/{orderTypeIdentifier}/{orderIdentifier}
```

## Path Parameters

`orderIdentifier`

`string`

 (Required) 

The order identifier. This value corresponds to the value of the `orderIdentifier` key of the Order.

`orderTypeIdentifier`

`string`

 (Required) 

The order type identifier of the order. This value corresponds to the value of the `orderTypeIdentifier` key of the Order.

## Header Parameters

`Authorization`

`string`

 (Required) 

The authentication for an order. The scheme is `AppleOrder` with the Order’s value for the `authenticationToken` key as parameter. For example, `AppleOrder {authenticationToken}`.

Value: `AppleOrder {authenticationToken}`

`If-Modified-Since`

`string`

If available, the most recent `If-Modified` value.

## Response Codes

` 200 ``OK`

`OK`

The request was successful and the response includes the Order data as payload.

Content-Type: application/vnd.apple.finance.order

` 304 ``Not Modified`

`Not Modified`

The request wasn’t modified since it was last loaded.

` 401 ``Request Not Authorized`

`Request Not Authorized`

The request isn’t authorized.

## Discussion

The device uses this endpoint for both initial and subsequent attempts to retrieve an order. Make sure you support standard HTTP caching on this endpoint.

## See Also

### Essentials

Creating the source for an order

Define an order by creating the directory structure, and adding source files and images.

Building a distributable order package

Prepare an order for distribution by building, signing, and compressing the source files.

Retrieve the registrations for a device

Retrieves the identifiers of the orders that the device registered for.

object Order

The order’s details, including information about the products or services rendered, customer service, and fulfillment.

Example Order Packages

Edit, build, and add example order packages to Wallet.


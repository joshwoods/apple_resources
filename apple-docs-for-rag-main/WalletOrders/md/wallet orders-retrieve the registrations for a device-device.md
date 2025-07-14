

- Wallet Orders
-  Retrieve the registrations for a device 

Web Service Endpoint

# Retrieve the registrations for a device

Retrieves the identifiers of the orders that the device registered for.

iOS 16.0+iPadOS 16.0+macOS 13.0+

## URL

``` source
GET https://your-web-service.com/v1/devices/{deviceIdentifier}/registrations/{orderTypeIdentifier}?ordersModifiedSince={lastModified}
```

## Path Parameters

`orderTypeIdentifier`

`string`

 (Required) 

The order type identifier of the order. This value corresponds to the value of the `orderTypeIdentifier` key of the Order.

`deviceIdentifier`

`string`

 (Required) 

A unique identifier used to recognize and authenticate the device.

## Query Parameters

`lastModified`

`string`

The value of the `lastModified` key from the response to a previous request. This value limits the results of the current request to the orders modified since the previous request.

## Response Codes

` 200 ``Matching Orders`

OrderIdentifiers

`Matching Orders`

The request was successful and the response includes the identifiers for the matching orders.

Content-Type: application/json

` 204 ``No Matching Orders`

`No Matching Orders`

There are no matching orders.

## See Also

### Essentials

Creating the source for an order

Define an order by creating the directory structure, and adding source files and images.

Building a distributable order package

Prepare an order for distribution by building, signing, and compressing the source files.

Retrieve the latest version of an order

Retrieves the latest signed and compressed version of an order.

object Order

The order’s details, including information about the products or services rendered, customer service, and fulfillment.

Example Order Packages

Edit, build, and add example order packages to Wallet.


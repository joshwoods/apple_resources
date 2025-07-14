

- App Store Connect API
-  Merchant ID 

API Collection

# Merchant ID

Manage your merchant ID for Apple Pay.

## Overview

Apple Pay developers and merchants can use this resource to automate registering both merchant ID and merchant name for interacting with Apple Pay services, and rotate required certificates to keep the service active. To learn more about developing and configuring Apple Pay, see Configure Apple Pay.

To learn more about setting up your Apple developer account and implementing Apple Pay in your apps, see Managing merchant IDs and Payment Processing certificates and Setting up Apple Pay.

Note

Apple Pay is not available for Enterprise teams.

## Topics

### Managing merchant IDs

Managing merchant IDs and Payment Processing certificates

Create and update certificates so your app uses Apple Pay and Wallet.

List merchant IDs

List all merchant Ids for your team.

Read details for a merchant ID

Get information for a merchant ID.

List certificates for a merchant ID

Get a list of all certificates for a specific merchant ID.

Modify merchant IDs

Update a specific merchant ID.

Create a merchant ID

Add a new merchant ID to your team.

Delete a merchant ID

Delete a specific merchant ID.

### Objects

object MerchantId

The data structure that represents a merchant ID resource.

object MerchantIdResponse

A response that contains a single merchant ID resource.

object MerchantIdsResponse

A response that contains a list of merchant ID resources.

object MerchantIdCreateRequest

The request body you use to create a merchant ID.

object MerchantIdUpdateRequest

The request body you use to update a merchant ID.

## See Also

### Provisioning

Bundle IDs

Manage the bundle IDs that uniquely identify your apps.

Bundle ID Capabilities

Manage the app capabilities for a bundle ID.

Certificates

Create, download, and revoke signing certificates for app development and distribution.

Devices

Register devices for development and testing.

Profiles

Create, delete, and download provisioning profiles that enable app installations for development and distribution.


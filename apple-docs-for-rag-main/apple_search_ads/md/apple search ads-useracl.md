

- Apple Search Ads
-  UserAcl 

Object

# UserAcl

The response to ACL requests.

Search Ads 2.0+

``` source
object UserAcl
```

## Properties

`currency`

`string`

The organization’s default currency that is set up in the Apple Search Ads UI.

Possible Values: `AUD, CAD, EUR, GBP, JPY, MXN, NZD, RUB, USD`

`orgId`

`int64`

The identifier of the organization that owns the campaign. Your `orgId` is the same as your account in the Apple Search Ads UI.

`orgName`

`string`

The name of your organization.

`parentOrgId`

`int64`

Distinguishes the account from an `orgId` belonging to a suborganization.

`paymentModel`

`string`

The payment model that you set through the Apple Search Ads UI. If you don’t set a payment model, campaigns can’t run.

`PAYG`  
A pay-as-you-go payment model.

`LOC`  
A line-of-credit payment model.

``  
There is no set payment method.

If you don’t select a payment model, you can still create campaigns. You must select a payment model before a campaign is eligible to run.

See Budget Orders for endpoints used to manage budget orders.

Possible Values: `LOC, PAYG`

`roleNames`

`[string]`

Each role governs what a user can see and do within the account:

API Account Manager  
Manage all campaigns within an account with read-and-write capabilities.

View reporting across the organization.

Create and edit an API public key.

API Account Read Only  
View reporting across the account with read-only permission.

Create and edit an API public key.

Limited Access  
API Read & Write:

View reporting.

Manage all campaigns and settings within a campaign group with read-and-write capabilities.

Create and edit an API public key.

Limited Access  
API Read Only:

View reporting across the organization.

Create and edit an API public key.

`timeZone`

`string`

The time zone you set during account creation through the Search Ads UI. `ORTZ`, the organization time zone, is the default.

## Mentioned in 

Apple Search Ads Campaign Management API 4

## See Also

### Access Control List

Get User ACL

Fetches roles and organizations that the API has access to.

object UserAclListResponse

A container for ACL call responses.

Get Me Details

Fetches details of an API caller.

object MeDetail

The API caller identifiers.

object MeDetailResponse

The response from me detail calls.


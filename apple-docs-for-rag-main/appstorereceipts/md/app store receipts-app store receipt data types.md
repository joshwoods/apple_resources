

- App Store Receipts
-  App Store receipt data types 

API Collection

# App Store receipt data types

Data types of objects that return in the receipt.

## Topics

### Transaction identifiers

type original_transaction_id

The transaction identifier of the original purchase.

Deprecated

type transaction_id

A unique identifier for a transaction, such as a purchase, restore, or renewal.

Deprecated

type app_account_token

The UUID that an app optionally generates to map a customer’s in-app purchase with its resulting App Store transaction.

Deprecated

### Receipt and subscription status

type status

The status of the app receipt.

Deprecated

type auto_renew_status

The renewal status for the auto-renewable subscription.

Deprecated

type is_in_billing_retry_period

An indicator of whether an auto-renewable subscription is in the billing retry period.

Deprecated

type is_in_intro_offer_period

An indicator of whether an auto-renewable subscription is in the introductory price period.

Deprecated

type is_trial_period

An indicator of whether an auto-renewable subscription is in the free trial period.

Deprecated

### Dates and intent

type expiration_intent

The reason a subscription expires.

Deprecated

type cancellation_date_ms

The time and date that the App Store refunds a transaction or revokes it from Family Sharing.

Deprecated

type expires_date_ms

The time, in milliseconds, a subscription expires or renews.

Deprecated

### Promotions and offers

type promotional_offer_id

The identifier of the promotional offer for an auto-renewable subscription that the user redeems.

Deprecated

type offer_code_ref_name

The offer-reference name of the subscription offer code that the customer redeems.

Deprecated

### Family Sharing

type in_app_ownership_type

The relationship of the user with the family-shared purchase to which they have access.

Deprecated


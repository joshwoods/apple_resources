

- Apple Pay on the Web
- ApplePayPayment
-  shippingContact 

Instance Property

# shippingContact

The shipping contact selected by the user for this transaction.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
ApplePayPaymentContact shippingContact;
```

## Discussion

The shipping contact information is populated if it is requested in ApplePayPaymentRequest. See ApplePayPaymentContact for the fields in shippingContact.

Shipping contact information can contain address, name, phone, and email fields. You determine which fields are present by setting the requiredShippingContactFields parameter in ApplePayPaymentRequest. Shipping contact details may differ based on the user’s geographic region.

Before the user authorizes the transaction with Touch ID, Face ID, or passcode, you receive redacted address information when onshippingcontactselected is triggered. Although the address is redacted for privacy, it includes sufficient information for you to compute taxes and shipping costs and refresh the corresponding values and total in the payment sheet.

Listing 1. Example of a redacted address in

```
{
"locality": "Cupertino",
"country": "United States",
"postalCode": "95014",
"administrativeArea": "CA",
"familyName": "",
"countryCode": "",
"givenName": ""
}
```

After the user authorizes the transaction, shippingContact contains the complete shipping contact data.

Listing 2. Example of after the user authorizes the transaction

```
{
"locality": "Cupertino",
"country": "United States",
"postalCode": "95014-2083",
"administrativeArea": "CA",
"emailAddress": "ravipatel@example.com",
"familyName": "Patel",
"addressLines": [
"1 Infinite Loop"
],
"givenName": "Ravi",
"countryCode": "US",
"phoneNumber": "(408) 555-5555"
}
```

Note

Address information can come from a wide range of sources and may be in a different format than you expect. Always validate the information before you use it.

## See Also

### Billing and shipping contacts

billingContact

The billing contact selected by the user for this transaction.

ApplePayPaymentContact

Contact information fields to use for billing and shipping contact information.




- Apple Pay on the Web
-  ApplePayPaymentContact 

Structure

# ApplePayPaymentContact

Contact information fields to use for billing and shipping contact information.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
dictionary ApplePayPaymentContact {
 DOMString phoneNumber;
 DOMString emailAddress;
 DOMString givenName;
 DOMString familyName;
 DOMString phoneticGivenName;
 DOMString phoneticFamilyName;
 sequence  addressLines;
 DOMString subLocality;
 DOMString locality;
 DOMString postalCode;
 DOMString subAdministrativeArea;
 DOMString administrativeArea;
 DOMString country;
 DOMString countryCode;
};
```

## Mentioned in 

Apple Pay on the Web Version 3 Release Notes

## Overview

The phoneticGivenName and phoneticFamilyName fields are available starting in Apple Pay version 3.

## Topics

### Contact properties

phoneNumber

A phone number for the contact.

emailAddress

An email address for the contact.

givenName

The contact’s given name.

familyName

The contact’s family name.

phoneticGivenName

The phonetic spelling of the contact’s given name.

phoneticFamilyName

The phonetic spelling of the contact’s family name.

### Address properties

addressLines

The street portion of the address for the contact.

subLocality

Additional information associated with the location, typically defined at the city or town level (such as district or neighborhood), in a postal address.

locality

The city for the contact.

postalCode

The zip code or postal code, where applicable, for the contact.

subAdministrativeArea

The subadministrative area (such as a county or other region) in a postal address.

administrativeArea

The state for the contact.

country

The name of the country or region for the contact.

countryCode

The contact’s two-letter ISO 3166 country code.

## See Also

### Providing known contact information

billingContact

Billing contact information for the user.

shippingContact

Shipping contact information for the user.


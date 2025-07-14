

- Security
- Certificate, Key, and Trust Services
- Trust
-  Usage Constraints Dictionary Keys 

API Collection

# Usage Constraints Dictionary Keys

Use these trust settings keys in a usage constraints dictionary.

## Topics

### Constants

var kSecTrustSettingsPolicy: String

A policy object specifying the certificate verification policy.

var kSecTrustSettingsApplication: String

A trusted application reference for the application checking the certificate’s trust settings.

var kSecTrustSettingsPolicyString: String

A string containing policy-specific data.

var kSecTrustSettingsKeyUsage: String

A number specifying the operations for which the encryption key in this certificate can be used.

var kSecTrustSettingsAllowedError: String

A number which, if encountered during certificate verification, is ignored for that certificate.

var kSecTrustSettingsResult: String

A number indicating the effective trust setting for this usage constraints dictionary.


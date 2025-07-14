

- Security
-  SecTrustSettingsCopyTrustSettings(\_:\_:\_:) 

Function

# SecTrustSettingsCopyTrustSettings(\_:\_:\_:)

Obtains the trust settings for a certificate.

Mac Catalyst 13.0+macOS 10.0+

``` source
func SecTrustSettingsCopyTrustSettings(
    _ certRef: SecCertificate,
    _ domain: SecTrustSettingsDomain,
    _ trustSettings: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`certRef`  

The certificate for which you want the trust settings. Pass the value kSecTrustSettingsDefaultRootCertSetting to obtain the default root certificate trust settings for the domain.

`domain`  

The domain from which you want to get trust settings. For possible values, see SecTrustSettingsDomain.

`trustSettings`  

On return, an array of CFDictionary objects that specify the trust settings for the certificate. For the contents of the dictionaries, see the discussion below. In Objective-C, call the CFRelease function to release this object when you’re finished with it.

## Return Value

A result code. See Security Framework Result Codes. Returns errSecItemNotFound if no trust settings exist for the specified certificate and domain.

## Discussion

The system expresses each certificate’s trust settings as a CFArray that includes any number (including zero) of dictionaries of type CFDictionary, each of which describes one set of usage constraints. Each usage-constraints dictionary may contain any of the following key-value pairs:

kSecTrustSettingsPolicy  
A policy object (SecPolicy) that specifies the certificate verification policy; for example: TLS or SMIME. Create a policy object using the `SecPolicyCreate` functions; for example, to create a standard TLS verification policy, use SecPolicyCreateSSL(_:_:).

kSecTrustSettingsApplication  
A trusted application reference (SecTrustedApplication) for the app that checks the certificate’s trust settings. Use the SecTrustedApplicationCreateFromPath(_:_:) function to get this reference.

kSecTrustSettingsPolicyString  
A CFString that contains policy-specific data. For an SMIME policy, this string contains an email address. For a TLS policy, it contains a host name.

kSecTrustSettingsKeyUsage  
A CFNumber that contains an `SInt32` value specifying the operations that can use the encryption key in this certificate. For possible values, see SecTrustSettingsKeyUsage.

kSecTrustSettingsResult  
A `CFNumber` that contains an `SInt32` value indicating the effective trust setting for this usage-constraints dictionary.

The system includes a usage-constraints dictionary in its evaluation of trust for a certificate only if the policy, application, and key use given in the dictionary match the use for which the system is evaluating the certificate. If this is the case, then the system combines the value of the `kSecTrustSettingsResult` key with the values from other matching dictionaries to determine the overall trust setting for the certificate, using a logical `OR` operation.

If this key isn’t present, the system assumes a default value of `kSecTrustSettingsResultTrustRoot`. Only a root certificate can have this value; therefore it’s invalid to create a usage-constraints dictionary for a non-root certificate without this key.

For the possible values for this key, see SecTrustSettingsResult.

kSecTrustSettingsAllowedError  
A CFNumber that contains an `SInt32` value indicating a `CSSM_RETURN` result code. If the system encounters this result code due to an error when it evaluates the trust for a certificate, it ignores the error.

The system applies this “allowed error” value to the certificate evaluation only if the usage-constraints dictionary meets the criteria described with the `kSecTrustSettingsResult` key. A usage-constraints dictionary with no constraints but with an allowed error value causes the system to always ignore that value when evaluating a certificate.

The system determines the overall trust settings for a certificate by combining the trust-settings results from all the usage-constraints dictionaries that match the use for which it’s evaluating the certificate. Trust settings for a given use apply if *any* of the dictionaries in the certificate’s trust-settings array matches the specified use.

If the value of the kSecTrustSettingsResult key is a value other than SecTrustSettingsResult.unspecified for a usage constraints-dictionary that has no constraints, the system uses the default value SecTrustSettingsResult.trustRoot. To specify a value for the kSecTrustSettingsAllowedError component without explicitly trusting or distrusting the associated certificate, set the value of the kSecTrustSettingsResult key to SecTrustSettingsResult.unspecified.

The `trustSettings` parameter can return a valid but empty CFArray. This empty trust-settings array means “always trust this certificate” with an overall trust setting for the certificate of SecTrustSettingsResult.trustRoot. However, an empty trust settings array isn’t the same as no trust settings, where the `trustSettings` parameter returns `NULL`. No trust-settings array means “this certificate must be verifiable using a known trusted certificate”.

Note

The trust settings result value SecTrustSettingsResult.trustRoot can only apply to root (self-signed) certificates. It’s an error to apply it to non-root certificates, including implicitly by using an empty trust settings array. Instead, use SecTrustSettingsResult.trustAsRoot.

### Special considerations

The system authenticates the person before making changes to per-user trust settings. On macOS 11 and later, the system authenticates the person as an administrator before making changes to system-wide trust settings. Therefore, you can only modify trust settings when running in a GUI environment; for example, a launch daemon can’t modify the settings.




- Security
- Certificate, Key, and Trust Services
-  Policies 

API Collection

# Policies

Obtain policies for establishing trust.

## Overview

For a certificate that is deemed intact and valid (because the chain of signatures is unbroken back to a trusted root certificate), you evaluate it against a set of rules known as a *trust policy*. The policy indicates how particular fields or extensions of a certificate affect whether it should be trusted for a particular use. For example, the policy may state that a certificate must not be expired or must be marked as valid for encryption, code signing, or some other specific purpose.

Usually you use a standard, predefined policy, such as the basic X509 policy or the SSL policy. You can also create custom policies with the certificate, key, and trust services API.

## Topics

### Standard Policies

func SecPolicyCreateBasicX509() -> SecPolicy

Returns a policy object for the default X.509 policy.

func SecPolicyCreateSSL(Bool, CFString?) -> SecPolicy

Returns a policy object for evaluating SSL certificate chains.

func SecPolicyCreateRevocation(CFOptionFlags) -> SecPolicy?

Returns a policy object for checking revocation of certificates.

Revocation Policy Constants

Use these flags to create a revocation policy object.

class SecPolicy

An object that represents a trust policy.

func SecPolicyGetTypeID() -> CFTypeID

Returns the unique identifier of the opaque type to which a policy object belongs.

### Advanced Policy Management

func SecPolicyCreateWithProperties(CFTypeRef, CFDictionary?) -> SecPolicy?

Returns a policy object based on an object identifier for the policy type.

func SecPolicyCopyProperties(SecPolicy) -> CFDictionary?

Returns a dictionary containing a policy’s properties.

Security Policy Keys

Use these dictionary keys to get and set policy properties.

Standard Policies for Specific Certificate Types

Use special OIDs to cause a certificate to be evaluated based on security policies specific to a given type of certificate.

### Legacy Symbols

class SecPolicySearch

An object that contains information about a policy search.


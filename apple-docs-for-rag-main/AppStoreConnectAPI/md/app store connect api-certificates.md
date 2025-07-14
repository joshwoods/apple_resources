

- App Store Connect API
-  Certificates 

API Collection

# Certificates

Create, download, and revoke signing certificates for app development and distribution.

## Overview

The `certificates` resource represents the digital certificates you use to sign your iOS or Mac apps for development and distribution. You can create new certificates, revoke existing certificates, and download certificates.

Note

You can only create Developer ID certificates for macOS through the Apple Developer website or Xcode. For more information, see Security.

## Topics

### Creating and modifying certificates

Create a Certificate

Create a new certificate using a certificate signing request.

Modify a certificate

Update the activation status for a specific certificate.

### Getting certificate infomation and data

List and Download Certificates

Find and list certificates and download their data.

Read and Download Certificate Information

Get information about a certificate and download the certificate data.

### Revoking certificates

Revoke a Certificate

Revoke a lost, stolen, compromised, or expiring signing certificate.

### Object and data types

object Certificate

The data structure that represents a Certificates resource.

object CertificatesWithoutIncludesResponse

object CertificateCreateRequest

The request body you use to create a Certificate.

object CertificateResponse

A response that contains a single Certificates resource.

object CertificatesResponse

A response that contains a list of Certificates resources.

object CertificateUpdateRequest

The request body you use to update a certificate activation status.

type CertificateType

Literal values that represent types of signing certificates.

## See Also

### Provisioning

Bundle IDs

Manage the bundle IDs that uniquely identify your apps.

Bundle ID Capabilities

Manage the app capabilities for a bundle ID.

Devices

Register devices for development and testing.

Profiles

Create, delete, and download provisioning profiles that enable app installations for development and distribution.

Merchant ID

Manage your merchant ID for Apple Pay.


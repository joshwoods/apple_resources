

- Enterprise Program API
-  Certificates 

API Collection

# Certificates

Create, download, and revoke signing certificates for app development and distribution.

## Overview

The `certificates` resource represents the digital certificates you use to sign your apps for development and distribution. You can create new certificates, revoke existing certificates, and download certificates.

Note

You can only create Developer ID certificates for macOS through the Apple Developer website or Xcode. For more information, see Security.

## Topics

### Creating Certificates

Create a Certificate

Create a new certificate using a certificate signing request.

### Getting Certificate Infomation and Data

List and Download Certificates

Find and list certificates and download their data.

Read and Download Certificate Information

Get information about a certificate and download the certificate data.

### Revoking Certificates

Revoke a Certificate

Revoke a lost, stolen, compromised, or expiring signing certificate.

### Object and Data Types

object Certificate

The data structure that represents a Certificates resource.

object CertificatesWithoutIncludesResponse

A response that contains a single certificate resource without includes.

object CertificateCreateRequest

The request body you use to create a Certificate.

object CertificateResponse

A response that contains a single Certificates resource.

object CertificatesResponse

A response that contains a list of Certificates resources.

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

Pass Type Ids

Create, download, and revoke pass type ids for app development and distribution.

Profiles

Create, delete, and download provisioning profiles for development and distribution.


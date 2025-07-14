

- ProximityReader
- MobileDriversLicenseDataRequest
- MobileDriversLicenseDataRequest.Response
- MobileDriversLicenseDataRequest.Response.DocumentElements
-  MobileDriversLicenseDataRequest.Response.DocumentElements.DHSComplianceStatus 

Enumeration

# MobileDriversLicenseDataRequest.Response.DocumentElements.DHSComplianceStatus

A type that represents the mobile driver’s license’ DHS (U.S. Department of Homeland Security) compliance status.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
enum DHSComplianceStatus
```

## Overview

This is also known as the document’s “REAL ID status”.

## Topics

### Operators

static func == (MobileDriversLicenseDataRequest.Response.DocumentElements.DHSComplianceStatus, MobileDriversLicenseDataRequest.Response.DocumentElements.DHSComplianceStatus) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case compliant

A constant that indicates the mobile driver’s license is DHS compliant.

case noncompliant

A constant that indicates the mobile driver’s license is not DHS compliant.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable


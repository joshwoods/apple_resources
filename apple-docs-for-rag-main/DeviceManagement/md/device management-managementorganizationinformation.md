

- Device Management
-  ManagementOrganizationInformation 

Object

# ManagementOrganizationInformation

The declaration to configure the managing organization’s contact information.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagementOrganizationInformation
```

## Properties

`Email`

`string`

The email address of the contact person for the organization.

`Name`

`string`

 (Required) 

The name of the organization.

`Proof`

ManagementOrganizationInformationProofObject

The additional properties that verify the identity and authenticity of the organization.

`URL`

`string`

The website of the organization to contact for support.

## Discussion

Specify `com.apple.management.organization-info` as the declaration type.

## Topics

### Supporting Objects

object ManagementOrganizationInformationProofObject

The additional properties that verify the identity and authenticity of the organization.

## See Also

### Management

object ManagementProperties

The declaration to configure the properties on the device.

object ManagementServerCapabilities

The declaration to configure the server’s feature set.


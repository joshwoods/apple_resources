

- Device Management
-  Configuring Multiple Devices Using Profiles 

Article

# Configuring Multiple Devices Using Profiles

Create and deploy configuration profiles to users within your organization.

## Overview

Configuration profiles streamline the process of setting up a large number of devices. Custom calendar and email settings, network settings (like WiFi and VPN settings), certificates, and device restrictions, are some of the properties you can configure using configuration profiles.

You have several options for deploying configuration profiles:

- Using Apple Configurator 2, available in the App Store.

- In an email message.

- On a webpage.

- Using over-the-air configuration as described in Over-the-Air Profile Delivery and Configuration.

- Over the air using a Mobile Device Management server.

Important

Configuration profiles are for enterprise use only. With the exceptions of the APN, VPN, and WiFi profiles, don’t use configuration profiles with consumer apps.

### Define a Profile

Configuration profiles are in a property list format, which any XML tool can read and write.

The configuration property list contains the properties listed in the TopLevel object. These properties describe the profile and the rules for deploying it. Specific configuration values are stored in an array of payloads in the `PayloadContent` property.

Each payload’s contents contain profile-specific keys (see Profile-Specific Payload Keys) and keys that are common to all payloads (see the following list of key definitions).

`PayloadType` (String)  
The payload type, specified on each payload domain’s reference page.

`PayloadVersion` (Integer)  
The version of this specific payload.

`PayloadIdentifier` (String)  
The reverse-DNS-style identifier for the payload. This identifier is usually the same as the TopLevel value, with an additional component appended.

`PayloadUUID` (String)  
The globally unique identifier for the payload. The actual content is unimportant, but must be globally unique. In macOS, use `uuidgen` to generate UUIDs.

`PayloadDisplayName` (String)  
The human-readable name for the profile payload. The name is displayed on the Detail screen and doesn’t have to be unique.

`PayloadDescription` (String)  
The human-readable description of this payload. This description is shown on the Detail screen.

`PayloadOrganization` (String)  
The human-readable string containing the name of the organization that provided the profile. This value doesn’t need to match the organization payload value in the enclosing dictionary.

### Encrypt and Sign a Profile

Both iOS and macOS support using encryption to protect the contents of profiles from unauthorized access. The encrypted profile can only be decrypted using a private key previously installed on a device. To encrypt a profile:

1.  Remove the `PayloadContent` array and serialize it as a property list. Note that the top-level object in this property list is an array, not a dictionary.

2.  CMS-encrypt the serialized property list as enveloped data.

3.  Serialize the encrypted data in DER (Distinguished Encoding Rules) format.

4.  Set the serialized data as the value of as a data property list item in the profile, using the `EncryptedPayloadContent` key.

Signing a profile guarantees data integrity. To sign a profile, place the XML property list in a DER-encoded, CMS Signed Data structure. When replacing a signed configuration profile, if you don’t sign the replacement using the exact same signing identity, the device rejects the replacement, unless installing the replacement through MDM or OTA.

### Example SCEP Configuration Profile

The listing below shows the contents of an example profile, containing a Simple Certificate Enrollment Protocol (SCEP) payload.

```

      PayloadVersion
      1
      PayloadUUID
      Ignored
      PayloadType
      Configuration
      PayloadIdentifier
      Ignored
      PayloadContent

            PayloadContent

               URL 
               https://scep.example.com/scep 
               Name 
               EnrollmentCAInstance 
               Subject

                        O
                        Example, Inc.

                        CN
                        User Device Cert

               Challenge
               ...
               Keysize
               1024
               KeyType
               RSA
               KeyUsage
               5

            PayloadDescription
            Provides device encryption identity 
            PayloadUUID 
            fd8a6b9e-0fed-406f-9571-8ec98722b713 
            PayloadType 
            com.apple.security.scep 
            PayloadDisplayName 
            Encryption Identity 
            PayloadVersion 
            1 
            PayloadOrganization 
            Example, Inc. 
            PayloadIdentifier 
            com.example.profileservice.scep 

```

## See Also

### Configuration Profiles

Profile-Specific Payload Keys

Use the appropriate payload for your configuration needs.


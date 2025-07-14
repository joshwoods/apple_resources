

- Device Management
-  Identification 

Device Management Profile

# Identification

The payload you use to configure the names of the account user.

macOS 10.7–15.4DeprecatedDevice Assignment ServicesVPP License Management

``` source
object Identification
```

## Properties

`PayloadIdentification`

Identification.PayloadIdentification

Deprecated   (Required) 

The dictionary that contains details about the user.

## Discussion

Specify `com.apple.configurationprofile.identification` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            CalDAVAccountDescription
            My CalDAV Account
            CalDAVHostName
            server.companyemail.com
            CalDAVPassword
            Password123
            CalDAVPort
            443
            CalDAVUseSSL

            CalDAVUsername
            juanchaves4@companyemail.com
            PayloadIdentifier
            com.example.mycaldavpayload
            PayloadType
            com.apple.caldav.account
            PayloadUUID
            603409f1-b611-459d-9584-0ed12bc25b5b
            PayloadVersion
            1

            PayloadIdentification

                UserName
                juanchaves4@companyemail.com
                FullName
                Juan Chavez
                EmailAddress
                juanchaves4@companyemail.com
                AuthMethod
                UserEnteredPassword
                Password
                Password123
                Prompt
                Prompt Hello
                PromptMessage
                Prompt Message

            PayloadType
            com.apple.configurationprofile.identification
            PayloadIdentifier
            com.example.myidentificationpayload
            PayloadUUID
            9afecc40-d89f-4d66-ba9a-73ce0f15f784
            PayloadVersion
            1

    PayloadDisplayName
    Identification with CalDAV
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    4a430145-e362-4808-957c-b784a1092777
    PayloadVersion
    1

```

## Topics

### Objects

object Identification.PayloadIdentification

The dictionary containing details about the user.

## See Also

### Authentication

object DirectoryService

The payload you use to configure an Active Directory (AD) domain.

object ExtensibleSingleSignOn

The payload you use to configure an app extension that performs single sign-on (SSO).

object ExtensibleSingleSignOnKerberos

The payload you use to configure an app extension that performs single sign-on with the Kerberos extension.

object IdentityPreference

The payload you use to configure the user’s identity on the device.

object SingleSignOn

The payload you use to configure single sign-on (SSO).


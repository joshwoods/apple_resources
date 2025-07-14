

- Device Management
-  EducationConfiguration 

Device Management Profile

# EducationConfiguration

The payload you use to configure the users, groups, and departments within an educational organization.

iOS 9.3+iPadOS 9.3+macOS 10.14+Device Assignment ServicesVPP License Management

``` source
object EducationConfiguration
```

## Properties

`Departments`

`[`EducationConfiguration.DepartmentsItem`]`

*For shared iPad profiles:* The array of dictionaries that defines which departments the system displays in the Shared iPad login screen. If set, the system uses this key to configure both Classroom and the Shared iPad login screen.

`DeviceGroups`

`[`EducationConfiguration.DeviceGroupsItem`]`

*For leader/teacher profiles:* The array of dictionaries that defines which device groups the leader can assign devices to. Not included in member payloads.

`Groups`

`[`EducationConfiguration.GroupsItem`]`

 (Required) 

*For shared iPad profiles:* The array of dictionaries that defines which groups the user can select in the login window.

*For leader/teacher profiles:* The array of dictionaries that defines the groups that the user can control.

*For member/student profiles:* The array of dictionaries that defines the groups where the user is a member.

`LeaderPayloadCertificateAnchorUUID`

`[string]`

The array of UUIDs referring to certificate payloads within the same profile that the system uses to authorize leader peer certificate identities. This array needs to contain all necessary certificates to validate the entire chain of trust. Leader certificates needs to have the common name prefix leader, which is case insensitive.

This property doesn’t support identity payloads or PKCS12 certificates.

Required when configuring a student device for Classroom, and ignored when configuring an instructor device. Has no effect on the configuration of the Shared iPad login screen.

`MemberPayloadCertificateAnchorUUID`

`[string]`

The array of UUIDs referring to certificate payloads within the same profile that the system uses to authorize group member peer certificate identities. This array must contain all certificates needed to validate the entire chain of trust. Member certificates must have the common name prefix member (case insensitive).

This property doesn’t support identity payloads or PKCS12 certificates.

Required when configuring a student device for Classroom, and ignored when configuring an instructor device. Has no effect on the configuration of the Shared iPad login screen.

`OrganizationName`

`string`

 (Required) 

The organization’s display name. The system displays this name in the iOS login screen.

`OrganizationUUID`

`string`

 (Required) 

The organization’s UUID identifier. This identifier can be any valid UUID. All teacher and student devices that need to communicate with one another must have the same organization UUID, particularly if they originated from different Device Enrollment Programs.

`PayloadCertificateUUID`

`string`

The UUID of an identity certificate payload within the same profile to use for performing client authentication with other devices. This property supports PKCS12 certificates.

Required to configure Classroom. Has no effect on the configuration of the Shared iPad login screen.

`ResourcePayloadCertificateUUID`

`string`

The UUID of an identity certificate payload within the same profile that the system uses to perform client authentication when fetching additional resources, such as student images.

If set, the system uses this key to configure both Classroom and the Shared iPad login screen. If not set, the system uses MDM client identity.

`ScreenObservationPermissionModificationAllowed`

`boolean`

If `true`, the system allows students enrolled in managed classes to modify their teacher’s permissions for screen observation on their device.

Default: `false`

`UserIdentifier`

`string`

 (Required) 

The unique string that identifies the user of this device within the organization.

Don’t set this value in payloads intended to configure the Shared iPad login screen.

`Users`

`[`EducationConfiguration.UsersItem`]`

 (Required) 

For shared iPad profiles: The array of dictionaries that define the users that the system displays in the iOS login window.

*For leader/teacher profiles:* The array of dictionaries that define users that are members of the teacher’s groups.

*For member/student profiles:* The array of dictionaries that needs to contain the definition of the user specified in the `UserIdentifier` key. With one-to-one member devices, this key should include only the device user and the teacher but not other class members.

## Discussion

Specify `com.apple.education` as the payload type.

In iOS, send this payload over the device channel. Additionally, the system requires supervision unless the payload only specifies as teacher configuration.

In macOS, send this payload over the user channel. The system supports student payloads in macOS 10.14.4 and later.

Additionally, configure:

- All identities as both SSL clients and servers

- All certificates with a key size of at least 2048 bits

- All certificates to use a hashing algorithm of SHA256 or stronger

- Leader certificates to have the common name prefix leader, which is case insensitive

- Member certificates to have the common name prefix member, which is case insensitive

- TLS server certificates issued on or after September 1, 2020 00:00 GMT/UTC to have a validity period greater than 398 days; see About Upcoming Limits on Trusted Certificates for more information.

### Profile Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS, Shared iPad |
| User Channel               | macOS            |
| Allow Manual Install       | iOS, macOS       |
| Requires Supervision       | \-               |
| Requires User Approved MDM | \-               |
| Allowed in User Enrollment | iOS, macOS       |
| Allow Multiple Payloads    | \-               |

### Profile Example

```

    PayloadContent

            Password
            Password123
            PayloadCertificateFileName
            TestServerCert.p12
            PayloadContent
            ExampleD
            PayloadDescription
            Adds a PKCS#12-formatted certificate
            PayloadDisplayName
            LeaderIdentity.p12
            PayloadIdentifier
            com.example.myedconfigpayload
            PayloadType
            com.apple.security.pkcs12
            PayloadUUID
            c149dafb-033f-4894-8add-e1056dc1c420
            PayloadVersion
            1

            PayloadCertificateFileName
            Cert.cer
            PayloadContent
            ExampleD
            PayloadDescription
            Adds a CA root certificate
            PayloadDisplayName
            leader: Catalyst Certificate
            PayloadIdentifier
            com.example.mycertpayload
            PayloadType
            com.apple.security.root
            PayloadUUID
            0391e29c-f10d-4803-a749-d04ef7f6a8fa
            PayloadVersion
            1

            OrganizationUUID
            24A9D6AC-9C34-45F3-B92F-88C4657204C9
            OrganizationName
            Example Inc.
            PayloadCertificateUUID
            8DBA6415-6F70-47FE-B0D2-C70B3D35B7A3
            LeaderPayloadCertificateAnchorUUID

                c2113db2-8ea9-456d-a2e7-e19f4a706b75

            MemberPayloadCertificateAnchorUUID

                82c3100d-e22c-42db-b70b-3b628992c757

            Departments

                    Name
                    Phonetics
                    Identifier
                    NotNeeded
                    GroupBeaconIDs

                        1
                        2
                        3

            Groups

                    BeaconID
                    1
                    Name
                    Phonetic Info Provided
                    LeaderIdentifiers

                        can

                    MemberIdentifiers

                        juan
                        mei
                        tom
                        bill

            Users

                    Identifier
                    tom
                    Name
                    tom clark
                    GivenName
                    tom
                    FamilyName
                    clark
                    PhoneticGivenName
                    tom
                    PhoneticFamilyName
                    clark
                    AppleID
                    tom
                    ImageURL
                    https://url.example.com.jpg
                    PasscodeType
                    four

                    Identifier
                    Juan
                    Name
                    Juan Chavez
                    GivenName
                    Juan
                    FamilyName
                    Chavez
                    PhoneticGivenName
                    Juan
                    PhoneticFamilyName
                    Chavez
                    AppleID
                    Juan
                    ImageURL
                    https://url.example.com.jpg2
                    PasscodeType
                    four

                    Identifier
                    mei
                    Name
                    mei chen
                    GivenName
                    mei
                    FamilyName
                    chen
                    PhoneticGivenName
                    Mei
                    PhoneticFamilyName
                    Chen
                    AppleID
                    mei
                    ImageURL
                    https://url.example.com.jpg.3
                    PasscodeType
                    six

                    Identifier
                    bill
                    Name
                    bill james
                    GivenName
                    bill
                    FamilyName
                    james
                    PhoneticGivenName
                    Bill
                    PhoneticFamilyName
                    James
                    AppleID
                    bill
                    ImageURL
                    https://url.example.com.jpg.4
                    PasscodeType
                    complex

            PayloadDescription
            Configures the EDU mode loginwindow.
            PayloadDisplayName
            EDU mode
            PayloadIdentifier
            com.example.myedconfigpayload
            PayloadType
            com.apple.education
            PayloadUUID
            9AD88C7B-7478-44D0-BEDD-4B1709002916
            PayloadVersion
            1

    PayloadDisplayName
    Education
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    2E4F6563-21DE-499B-B834-4BCF1F08B5AD3
    PayloadVersion
    1

```

## Topics

### Objects

object EducationConfiguration.DepartmentsItem

A department in the organization.

object EducationConfiguration.DeviceGroupsItem

A device group in the organization.

object EducationConfiguration.GroupsItem

An array of dictionaries defining groups.

object EducationConfiguration.UsersItem

A user in the organization.

## See Also

### Managed Devices

object LightsOutManagementLOM

The payload you use to configure lights-out management (LOM) settings.

object ManagedPreferences

The payload you use to configure managed preferences.

object MDM

The payload you use to configure mobile device management (MDM) settings.

object ProfileRemovalPassword

The payload you use to configure profile removal.


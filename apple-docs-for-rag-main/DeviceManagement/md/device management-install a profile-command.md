

- Device Management
-  Install a Profile 

Web Service Endpoint

# Install a Profile

Install a configuration profile on a device.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#InstallProfileCommand
```

## HTTP Body

InstallProfileCommand

The command to install a configuration profile on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

InstallProfileResponse

`OK`

A response from the device after it processes the command to install a configuration profile.

Content-Type: application/xml

## Mentioned in 

Deploying MDM Enrollment Profiles

## Discussion

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS, Shared iPad                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Required Access Right      | AllowInstallationRemoval               |

### Example Request and Response

- Request
- Response

```

    Command

        Payload

        PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4KPCFET0NUWVBFIHBs
        aXN0IFBVQkxJQyAiLS8vQXBwbGUvL0RURCBQTElTVCAxLjAvL0VOIiAiaHR0cDovL3d3
        dy5hcHBsZS5jb20vRFREcy9Qcm9wZXJ0eUxpc3QtMS4wLmR0ZCI+CjxwbGlzdCB2ZXJz
        aW9uPSIxLjAiPgo8ZGljdD4KCTxrZXk+UGF5bG9hZENvbnRlbnQ8L2tleT4KCTxhcnJh
        eT4KCQk8ZGljdD4KCQkJPGtleT5QYXlsb2FkRGVzY3JpcHRpb248L2tleT4KCQkJPHN0
        cmluZz5Db25maWd1cmVzIHJlc3RyaWN0aW9uczwvc3RyaW5nPgoJCQk8a2V5PlBheWxv
        YWREaXNwbGF5TmFtZTwva2V5PgoJCQk8c3RyaW5nPlJlc3RyaWN0aW9uczwvc3RyaW5n
        PgoJCQk8a2V5PlBheWxvYWRJZGVudGlmaWVyPC9rZXk+CgkJCTxzdHJpbmc+Y29tLmFw
        cGxlLmFwcGxpY2F0aW9uYWNjZXNzLkVENzE2QUU5LUFFODktNENFQy1BNzE3LUYyMTU2
        N0UwRjUxMjwvc3RyaW5nPgoJCQk8a2V5PlBheWxvYWRUeXBlPC9rZXk+CgkJCTxzdHJp
        bmc+Y29tLmFwcGxlLmFwcGxpY2F0aW9uYWNjZXNzPC9zdHJpbmc+CgkJCTxrZXk+UGF5
        bG9hZFVVSUQ8L2tleT4KCQkJPHN0dmluZz5FRDcxNkFFOS1BRTg5LTRDRUMtQTcxNy1G
        MjE1NjdFMEY1MTI8L3N0cmluZz4KCQkJPGtleT5QYXlsb2FtVmVyc2lvbjwva2V5PgoJ
        CQk8aW50ZWdlcj4xPC9pbnRlZ2VyPgoJCQk8a2V5PmFsbG93TG9ja1NjcmVlblRvZGF5
        Vmlldzwva2V5PgoJCQk8ZmFsc2UvPgoJCQk8a2V5PnJhdGluZ1JlZ2lvbjwva2V5PgoJ
        CQk8c3RyaW5nPnVzPC9zdHJpbmc+CgkJPC9kaWN0PgoJPC9hcnJheT4KCTxrZXk+UGF5
        bG9hZERpc3BsYXlOYW1lPC9rZXk+Cgk8c3RyaW5nPihVKSBhbGxvd0xvY2tTY3JlZW5U
        b2RheVZpZXc8L3N0cmluZz4KCTxrZXk+UGF5bG9hZElkZW50aWZpZXI8L2tleT4KCTxz
        dHJpbmc+Y29tLmFwcGxlLmRtcy5yZXN0cmljdGlvbnMuYWxsb3dMb2NrU2NyZWVuVG9k
        YXlWaWV3PC9zdHJpbmc+Cgk8a2V5PlBheWxwYWRSZW1vdmFsRGlzYWxsb3dlZDwva2V5
        PgoJPGZhbHNlLz4KCTxrZXk+UGF5bG9hZFR5cGU8L2tleT4KCTxzdHJpbmc+Q29uZmln
        dXJhdGlvbjwvc3RyaW5nPgoJPGtleT5QYXlsb2FkVVVJRDwva2V5PgoJPHN0cmluZz42
        OUE0RTVGRS03NUQxLTQyOTctQkQzMi01NDA3MTBFRDYzNjA8L3N0cmluZz4KCTxrZXk+
        UGF5bG9hZFZlcnNpb248L2tleT4KCTxpbnRlZ2VyPjE8L2ludGVnZXI+CjwvZGljdD4K
        PC9wbGlzdD4K

        RequestType
        InstallProfile

    CommandUUID
    0001_InstallProfile

```

```

    CommandUUID
    0001_InstallProfile
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object InstallProfileCommand

The command to install a profile on a device.

object InstallProfileResponse

A response from the device after it processes the command to install a configuration profile.

## See Also

### Profile Management

List the Installed Profiles

Get a list of installed profiles on a device.

Remove a Profile

Remove a previously installed profile from the device.

Install a Provisioning Profile

Install a provisioning profile on a device.

List the Installed Provisioning Profiles

Get a list of installed provisioning profiles on a device.

Remove a Provisioning Profile

Remove a previously installed provisioning profile from a device.


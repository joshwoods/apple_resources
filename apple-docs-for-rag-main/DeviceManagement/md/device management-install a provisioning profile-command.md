

- Device Management
-  Install a Provisioning Profile 

Web Service Endpoint

# Install a Provisioning Profile

Install a provisioning profile on a device.

iOS 4.0+iPadOS 4.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

## URL

``` source
PUT https://yourmdmhost.example.com/mdm#InstallProvisioningProfileCommand
```

## HTTP Body

InstallProvisioningProfileCommand

The command to install a provisioning profile on a device.

Content-Type: application/x-apple-aspen-mdm

## Response Codes

` 200 ``OK`

InstallProvisioningProfileResponse

`OK`

A response from the device after it processes the command to install a provisioning profile.

Content-Type: application/xml

## Mentioned in 

Installing Profiles on Devices

## Discussion

No error occurs if the provisioning profile is already present.

Refer to the following sections to determine supported channels and requirements, and to see an example request and response.

### Command Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Requires Supervision       | \-                                     |
| Allowed in User Enrollment | iOS                                    |
| Required Access Right      | AllowProvisioningInstallationRemoval   |

### Example Request and Response

- Request
- Response

```

    Command

        ProvisioningProfile

        TG9yZW0gaXBzdW0gZG9sb3Igc2l0IGFtZXQsIGNvbnNlY3RldHVyIGFkaXBpc2Npbmcg
        ZWxpdC4gTWF1cmlzIGlwc3VtIGVyYXQsIHNlbXBlciBxdWlzIG1hc3NhIG5lYywgcHVs
        dmluYXIgcHVsdmluYXIgbWF1cmlzLiBBbGlxdWFtIGNvbW1vZG8gaWQgdXJuYSBzZWQg
        Y29uc2VxdWF0LiBEb25lYyBlZ2V0IGFsaXF1ZXQgYXVndWUuIEZ1c2NlIHF1aXMgdG9y
        dG9yIHZlbGl0LiBFdGlhbSBhdWN0b3IgdmVsIG1hc3NhIHNpdCBhbWV0IG1vbGxpcy4g
        TmFtIGVsZW1lbnR1bSB2aXRhZSBuZXF1ZSBhYyBhY2N1bXNhbi4gVml2YW11cyBpZCBs
        ZW8gYXVndWUuIFByb2luIGlhY3VsaXMgdWxsYW1jb3JwZXIgc2VtLCB2ZWwgZGFwaWJ1
        cyBvcmNpIGNvbnNlcXVhdCBzaXQgYW1ldC4gQ3JhcyBhYyBtb2xlc3RpZSBleC4KCklu
        IG1vbGVzdGllIGJpYmVuZHVtIG1hZ25hIGlkIHVsdHJpY2VzLiBOYW0gZmF1Y2lidXMg
        anVzdG8gbmVjIGZlbGlzIHB1bHZpbmFyIGZhY2lsaXNpcy4gQ3JhcyBjb21tb2RvLCBk
        aWFtIGluIHRpbmNpZHVudCB1bHRyaWNlcywgcXVhbSBlbmltIHNvbGxpY2l0dWRpbiB0
        dXJwaXMsIGV1IHRpbmNpZHVudCBuaXNpIGxvcmVtIGV0IGxpZ3VsYS4gU3VzcGVuZGlz
        c2UgcG90ZW50aS4gVmVzdGlidWx1bSBuZWMgbWFnbmEgZXUgbWV0dXMgbWF4aW11cyB1
        bHRyaWNlcyBhIGNvbnZhbGxpcyBvcmNpLiBDcmFzIHF1aXMgdHVycGlzIHNvZGFsZXMs
        IHZhcml1cyBmZWxpcyBzZWQsIHNhZ2l0dGlzIG1hc3NhLiBQcmFlc2VudCBmZXJtZW50
        dW0gbnVsbGEgZXUgbnVsbGEgcGhhcmV0cmEgY29tbW9kby4gSW50ZWdlciB1dCBkYXBp
        YnVzIG5pc2kuIE51bGxhIHZlaGljdWxhIHV0IGVsaXQgc2VkIHZlbmVuYXRpcy4gRG9u
        ZWMgZXQgZWdlc3RhcyBhbnRlLiBJbnRlcmR1bSBldCBtYWxlc3VhZGEgZmFtZXMgYWMg
        YW50ZSBpcHN1bSBwcmltaXMgaW4gZmF1Y2lidXMuIE1hZWNlbmFzIHJob25jdXMgbmlz
        aSByaXN1cywgZXQgc29kYWxlcyB2ZWxpdCB2b2x1dHBhdCBhdC4KClF1aXNxdWUgdmVo
        aWN1bGEgZXJvcyBlZmZpY2l0dXIgc2FwaWVuIGx1Y3R1cywgYSByaG9uY3VzIG51bGxh
        IHZlc3RpYnVsdW0uIFNlZCBzZW1wZXIganVzdG8gbm9uIHRyaXN0aXF1ZSBsb2JvcnRp
        cy4gUGhhc2VsbHVzIGV0IGVyYXQgZXQgbmliaCB2aXZlcnJhIHZvbHV0cGF0IGlkIHZl
        bCBtYXNzYS4gUGhhc2VsbHVzIHNlZCBhdWd1ZSBhIGVzdCBydXRydW0gZWZmaWNpdHVy
        LiBWaXZhbXVzIHZ1bHB1dGF0ZSBzY2VsZXJpc3F1ZSBydXRydW0uIE1hdXJpcyBwb3J0
        YSBzYXBpZW4gdmVsIHNlbXBlciBzZW1wZXIuIEluIGhhYyBoYWJpdGFzc2UgcGxhdGVh
        IGRpY3R1bXN0LgoKQWxpcXVhbSBwb3J0dGl0b3Igbm9uIG1hc3NhIGVnZXQgY29uc2Vj
        dGV0dXIuIER1aXMgZWxlbWVudHVtIGxhY2luaWEgdG9ydG9yLCBhYyBwdWx2aW5hciBz
        ZW0gcGhhcmV0cmEgc2VkLiBJbnRlZ2VyIHJ1dHJ1bSBhdWd1ZSBlc3QsIGEgcmhvbmN1
        cyBuaXNpIGNvbnZhbGxpcyBlZ2V0LiBDcmFzIGFjY3Vtc2FuIGZlbGlzIGlwc3VtLCBu
        ZWMgdml2ZXJyYSBuaXNpIGZpbmlidXMgbmVjLiBGdXNjZSBhdCBsdWN0dXMgc2FwaWVu
        LCBzZWQgdGluY2lkdW50IGVzdC4gUGVsbGVudGVzcXVlIGFsaXF1ZXQgYXVjdG9yIGRh
        cGlidXMuIE1hZWNlbmFzIGVnZXQgZHVpIHRlbXB1cywgbW9sbGlzIGxvcmVtIGVnZXQs
        IHZ1bHB1dGF0ZSBkdWkuIEluIGV1IGxpYmVybyBhcmN1LiBDcmFzIG1hdHRpcyBldWlz
        bW9kIG5pYmgsIGF0IHNlbXBlciBvZGlvIGRhcGlidXMgaW4uCgpEb25lYyB2ZWwgc29k
        YWxlcyBkb2xvci4gTWFlY2VuYXMgbWFsZXN1YWRhIGhlbmRyZXJpdCBuaXNpIHF1aXMg
        ZmVybWVudHVtLiBDcmFzIG5vbiBjb25kaW1lbnR1bSBsZWN0dXMuIFV0IGZhY2lsaXNp
        cyBmZWxpcyB2YXJpdXMgZXJhdCBhY2N1bXNhbiB2ZWhpY3VsYS4gTW9yYmkgbHVjdHVz
        IHRvcnRvciB2ZWwgYW50ZSBwb3N1ZXJlLCBldCBwb3J0YSBhdWd1ZSBwb3N1ZXJlLiBT
        dXNwZW5kaXNzZSBlZ2VzdGFzIGVmZmljaXR1ciB2ZW5lbmF0aXMuIE51bmMgZnJpbmdp
        bGxhIGVyb3MgdXQgb2RpbyB2dWxwdXRhdGUgcG9zdWVyZS4gTmFtIGVzdCBkaWFtLCBz
        Y2VsZXJpc3F1ZSBtb2xlc3RpZSBvZGlvIHNlZCwgbHVjdHVzIG1vbGVzdGllIHRvcnRv
        ci4gTWF1cmlzIG9ybmFyZSBuZXF1ZSBpZCBpbnRlcmR1bSB0cmlzdGlxdWUuIFZpdmFt
        dXMgdXQgcHVydXMgdmFyaXVzLCBwb3J0dGl0b3IgbG9yZW0gZXQsIGZhdWNpYnVzIGFu
        dGUuIE51bGxhbSBub24gZGljdHVtIGFudGUuIFBlbGxlbnRlc3F1ZSB2dWxwdXRhdGUg
        dHVycGlzIGF0IGFjY3Vtc2FuIHZvbHV0cGF0LiBEb25lYyBub24gbGliZXJvIGF0IGVu
        aW0gdWxsYW1jb3JwZXIgYWxpcXVldC4gTmFtIGRpY3R1bSBkb2xvciBub24gZHVpIHRp
        bmNpZHVudCBtYWxlc3VhZGEuIFV0IGNvbnZhbGxpcyBlbGl0IGF0IG1pIGRpZ25pc3Np
        bSwgYWMgdWxsYW1jb3JwZXIgZmVsaXMgaW1wZXJkaWV0LiBOYW0gbm9uIHRyaXN0aXF1
        ZSBsZWN0dXMu

        RequestType
        InstallProvisioningProfile

    CommandUUID
    0001_InstallProvisioningProfile

```

```

    CommandUUID
    0001_InstallProvisioningProfile
    Status
    Acknowledged
    UDID
    00008020-000915083C80012E

```

## Topics

### Command and Response

object InstallProvisioningProfileCommand

The command to install a provisioning profile on a device.

object InstallProvisioningProfileResponse

A response from the device after it processes the command to install a provisioning profile.

## See Also

### Profile Management

Install a Profile

Install a configuration profile on a device.

List the Installed Profiles

Get a list of installed profiles on a device.

Remove a Profile

Remove a previously installed profile from the device.

List the Installed Provisioning Profiles

Get a list of installed provisioning profiles on a device.

Remove a Provisioning Profile

Remove a previously installed provisioning profile from a device.




- Device Management
- App and Book Management
- App and Book Management (Legacy)
-  Upgrading to Apple School Manager (ASM) and Apple Business Manager (ABM) 

Article

# Upgrading to Apple School Manager (ASM) and Apple Business Manager (ABM)

Manage devices and content across an organization user base with a single destination.

## Overview

Apple School Manager (ASM) and Apple Business Manager (ABM) enable content managers to purchase content in the same place that they manage Apple IDs and devices. You can automate device deployment, purchase and distribute content, and manage roles in your organization. Working seamlessly with your mobile device management (MDM) solution, ASM and ABM make it easy to enroll devices, deploy content, and delegate administrative privileges.

### Upgrading to support location-based tokens

The purchases made in VPP in ASM and ABM are location-based, making it easy for content managers to move licenses between locations as needed. Upgrading to location-based tokens in ASM or ABM is strongly recommended, but optional. Update your MDM to support location-based tokens as follows:

1.  Update API calls to handle the `location` field being returned. Licenses assigned with a legacy token will not have a location. All assets purchased with VPP in ASM or ABM will have an additional `location` field in their API responses.

2.  Update the MDM UI to show location names for tokens and assets. Location names are not unique (many schools may have the same name) but location UIDs are unique to a specific location. Displaying the location name to the user is particularly important when the location token is about to expire.

3.  Refresh license status at appropriate times (each page load) to maintain an accurate UI. Since licenses can be reallocated in ASM and ABM, license counts will change outside of the MDM.

4.  Use Get Assets not Get Licenses to get license counts. Get Assets is more efficient and will return an aggregation of `adamId` values and counts, instead of all the individual licenses.

5.  Handle the case when duplicate tokens are uploaded by different content managers. There is just one location token that needs to be stored, instead of a token per VPP account.

    The `uId` field is a unique library identifier which is included in all API responses. When querying assets using multiple tokens that may share libraries, use the `uId` field to filter duplicates.

6.  Handle any new errors related to location-based tokens. See Interpreting Error Codes for more information.

Warning

Licenses which have been assigned using a legacy token must continue to be managed by the legacy token until they are transferred to a location. MDMs will need to support both models of licensing simultaneously. Failure to support both the legacy and location based models of tokens will create discrepancies between user experiences in ASM/ABM and their MDM.

## See Also

### Getting Started

Managing Apps and Books Through Web Services

Associate volume purchases with users or devices using endpoints for Mobile Device Management (MDM), provided by the Volume Purchase Program (VPP).

Interpreting Error Codes

Investigate service request errors and troubleshoot solutions.


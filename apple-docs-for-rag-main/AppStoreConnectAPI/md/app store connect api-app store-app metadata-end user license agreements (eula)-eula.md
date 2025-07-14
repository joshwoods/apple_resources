

- App Store Connect API
- App Store
- App Metadata
-  End User License Agreements (EULA) 

API Collection

# End User License Agreements (EULA)

Manage custom End User License Agreements (EULA) that are related to territories.

## Overview

`endUserLicenseAgreements` represents the custom End User License Agreement (EULA) that you provide. Apple provides a standard EULA that applies in all territories. If you need to provide a custom EULA, use this resource to provide your agreement text. Relate it to the app and territories for which it applies using the Territories resource.

For more information, see App Store Connect Help: Create a new version.

## Topics

### Creating, Modifying, and Deleting an EULA

Create an End User License Agreement

Add a custom end user license agreement (EULA) to an app and configure the territories to which it applies.

Modify an End User License Agreement

Update the text or territories for your custom end user license agreement.

Delete an End User License Agreement

Delete the custom end user license agreement that is associated with an app.

### Reading EULA and Listing Territories

Read End User License Agreement Information

Get the custom end user license agreement associated with an app, and the territories it applies to.

Read the End User License Agreement Information of an App

Get the custom end user license agreement (EULA) for a specific app and the territories where the agreement applies.

List All Territories for an End User License Agreement

List all the App Store territories to which a specific custom app license agreement applies.

### Objects

object EndUserLicenseAgreement

The data structure that represents the End User License Agreement resource.

object EndUserLicenseAgreementCreateRequest

The request body you use to create an End User License Agreement.

object EndUserLicenseAgreementUpdateRequest

The request body you use to update an End User License Agreement.

object EndUserLicenseAgreementResponse

A response that contains a single End User License Agreements resource.

object EndUserLicenseAgreementWithoutIncludesResponse




- App Store Connect API
- App Store
-  App Clips and App Clip Experiences 

# App Clips and App Clip Experiences

Read App Clip information and manage App Clip experiences.

## Overview

Creating and managing default and advanced App Clip experiences using the App Store Connect website are key tasks when creating an App Clip. However, your App Clip may require many App Clip experiences. For example, your App Clip could allow users to order food at a chain restaurant with hundreds of locations. Each location would need its own advanced App Clip experience to display a photo of the location on the App Clip card. To reduce the effort of managing hundreds or even thousands of App Clip experiences, use the App Store Connect API to automatically access App Clip information and automate the creation and management of:

- Default App Clip experiences

- Advanced App Clip experiences

- App Clip experiences for testers

If you’re new to creating an App Clip, see App Clips and Human Interface Guidelines > App Clips. For more information about creating App Clip experiences, see Configuring the launch experience of your App Clip.

### Review App Store Connect API Usage

To read App Clip information and manage App Clip experiences with the App Store Connect API, you need to understand key concepts for using the API. If you’re new to using the App Store Connect API, make sure to read the documentation in the Essentials section of App Store Connect API and learn how to create API keys, generate JWTs, identify rate limits, and more.

To read App Clip information and manage App Clip experiences, be sure you have one of the following user roles:

- `ACCOUNT_HOLDER`

- `ADMIN`

- `APP_MANAGER`

- `MARKETING`

For the full list of App Store Connect user roles, see UserRole.

Note

You need to create an App Clip and upload it to App Store Connect before you can create an App Clip experience using the App Store Connect API.

### Plan App Clip Experience Creation and Management

Creating or managing App Clip experiences typically requires a sequence of calls to endpoints the App Store Connect API provides. Before you start working on the implementation, list the steps required to achieve your goal. While the exact API calls you need to make depend on your use case, creating an App Clip experience usually involves:

1.  Gathering additional information

2.  Uploading the image asset that appears on the App Clip card

3.  Creating the App Clip experience

### Gather Required Information

Before you can create or update an App Clip experience using the App Store Connect API, you likely need to gather additional information. To find out what information you need:

1.  Identify the endpoint you need to call. For example, you use the Create a Default App Clip Experience endpoint to create a default App Clip experience.

2.  Review attributes and relationships of the request you send to the endpoint and other involved objects. For example, successfully creating a default App Clip experience requires App Clips, App Store Versions, App Clip App Store review details, App Clip Header Images, and Default App Clip Experience Localizations information.

### Upload the Image Asset that Appears on the App Clip Card

App Clip experience functionality provided by the App Store Connect API often involves uploading image assets to App Store Connect. For example, creating an App Clip experience using the App Store Connect API requires an image asset that appears on the App Clip card.

Uploading an image asset for an App Clip experience works similarly to uploading other assets to App Store Connect:

1.  Reserve the image asset using the Create an App Clip Card Image for a Default App Clip Experience endpoint for a default App Clip experience or the Create an App Clip Card Image for an Advanced App Clip Experience endpoint for an advanced App Clip experience.

2.  Upload the image asset using the upload operations provided in the response to your reservation request.

3.  Commit the image asset using the Modify an App Clip Card Image endpoint for a default App Clip experience and the Modify the Image for an Advanced App Clip Experience endpoint for an advanced App Clip experience.

4.  Fetch information about the image asset to verify that the upload succeeded using the Read the App Clip Card Image and Read Image Information for an Advanced App Clip Experience endpoints.

For additional information on uploading assets to App Store Connect, see Uploading Assets to App Store Connect.

### Create an App Clip Experience

Creating default and advanced App Clip experiences is a key functionality that App Store Connect provides. When you’ve gathered all required information and uploaded the image that appears on the App Clip card, you’re ready to create an App Clip experience.

To create a default App Clip experience:

- Call the Create a Default App Clip Experience endpoint. Be sure to attach the default App Clip experience to an App Store version by including the related App Store Versions resource in the AppClipDefaultExperienceCreateRequest. Alternatively, update an App Store Versions resource to include the new default App Clip experience.

- Call the Create App Store Review Details for an App Clip endpoint to provide the default App Clip experience’s invocation URL to App Review.

- Call the Create the Localized Metadata for a Default App Clip Experience endpoint to provide a localized subtitle and an image that appears on the App Clip card.

Tip

To create a new App Clip experience that uses metadata of an existing default App Clip experience, create the new experience and include the `appClipDefaultExperienceTemplate` relationship in the AppClipDefaultExperienceCreateRequest.

To create an advanced App Clip experience:

- Call the Create an Advanced App Clip Experience endpoint.

- Include the related App Clips, AppClipAdvancedExperienceLocalization, and Advanced App Clip Experience Images resources.

Important

For both default or advanced App Clip experiences, provide at least one localization and make sure that it matches your app’s primary locale. If your app supports additional localizations, provide the same localizations for each App Clip experience.

To create an advanced App Clip experience that appears in Apple Maps, you create an AppClipAdvancedExperienceCreateRequest.Data.Attributes.Place association that connects the App Clip experience to a physical location. Apple Maps uses any location data that you provide solely for matching an App Clip experience to an existing location. If it can’t find a match, Apple Maps doesn’t use the provided location data.

### Update and Delete App Clip Experiences

Similar to how App Store Connect provides functionality to create App Clip experiences, it also offers functionality to update App Clip experiences. For example, you may need to update the phone number of an advanced App Clip experience, or change the localized subtitle that appears on the App Clip card of a default App Clip experience. However, you can’t update existing App Clip experiences for an already released App Clip. To update an already released App Clip, create a new App Clip experience and attach it to a new version of your app. When the new version passes App Review and you publish it on the App Store, it uses the new App Clip experience.

Similarly, you can’t delete App Clip experiences for an already released app version unless you release a new version of your app without an App Clip. That said, you can use functionality provided by the Default App Clip Experiences and Advanced App Clip Experiences resources to update or delete App Clip experiences that aren’t attached to a released App Clip:

- To update a default App Clip experience, use the Modify a Default App Clip Experience endpoint.

- To delete a default App Clip experience, use the Delete a Default App Clip Experience endpoint.

- To update an advanced App Clip experience, use the Modify and Delete an Advanced App Clip Experience endpoint.

- To delete an advanced App Clip experience, use the Modify and Delete an Advanced App Clip Experience endpoint and set the `isPoweredBy` attribute of the AppClipAdvancedExperienceUpdateRequest to `true`.

### Manage Beta App Clip Experiences

Verifying that the launch experience of the App Clip is free of errors is a key task when developing an App Clip. When you distribute your full app with TestFlight, you can configure beta App Clip experiences that testers use to launch your App Clip with the TestFlight app. To help automate creating and updating beta App Clip experiences, use the Beta App Clip Invocations resource. It provides functionality to create, read, update, and delete a beta App Clip experience. For example, use the Create an App Clip Invocation for Testers in TestFlight endpoint to create a beta App Clip experience.

## Topics

### Getting App Clip and App Clip Experience Information

App Clips

Read App Clip and App Clip experience information.

### Managing App Clip Experiences

Default App Clip Experiences

Read, create, update, and delete your default App Clip experience.

Advanced App Clip Experiences

Create, read, update, and delete your advanced App Clip experiences.


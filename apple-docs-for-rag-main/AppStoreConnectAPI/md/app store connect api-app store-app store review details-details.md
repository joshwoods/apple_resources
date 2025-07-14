

- App Store Connect API
- App Store
-  App Store review details 

API Collection

# App Store review details

Manage the required information you provide for App Review.

## Overview

Use `appStoreReviewDetails` to provide information required for App Review. This information isn’t displayed on the App Store. Required attributes for App Review are:

- Contact first and last name

- Contact phone number

- Contact email address

- Whether testing your app requires a demo account

- Demo account name (if your app uses a single sign-on service)

- Demo account password (if your app uses a single sign-on service)

Optionally, provide notes for the review team using the notes attribute. If you need to attach a file for App Review, use the App Store review attachments resource.

For more information see App Review information.

## Topics

### Creating, Modifying, and Reading Review Details

Create an App Store Review Detail

Add App Store review details to an App Store version, including contact and demo account information.

Read App Store Review Detail Information

Get App Review details you provided, including contact information, demo account, and notes.

Modify an App Store Review Detail

Update the app store review details, including the contact information, demo account, and notes.

### Objects

object AppStoreReviewDetail

The data structure that represent an App Store Review Details resource.

object AppStoreReviewDetailCreateRequest

The request body you use to create an App Store Review Detail.

object AppStoreReviewDetailUpdateRequest

The request body you use to update an App Store Review Detail.

object AppStoreReviewDetailResponse

A response that contains a single App Store Review Details resource.

## See Also

### App Store Review Submissions

Review submissions

Create and manage your submissions for review, which can include your App Store version, App Store version experiments, custom product page versions, and in-app events.

Review submission items

Manage the contents of your review submission, which can include your App Store version, App Store version experiments, custom product page versions, and in-app events.

App Clip App Store review details

Manage required App Clip information you provide for App Review.

App Store review attachments

Manage the attachments you upload to App Store Connect for App Review.

App Store version submissions

Submit versions of your app to App Review.

Actors

Get information about who or which service made a review submission.


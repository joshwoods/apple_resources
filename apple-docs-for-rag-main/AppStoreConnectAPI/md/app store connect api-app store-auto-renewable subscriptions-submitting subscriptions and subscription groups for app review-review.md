

- App Store Connect API
- App Store
- Auto-Renewable Subscriptions
-  Submitting subscriptions and subscription groups for App Review 

Article

# Submitting subscriptions and subscription groups for App Review

Learn how to prepare and submit your subscriptions, subscription groups, and subscription screenshots for the App Review process with the App Store Connect API.

## Overview

After you create and configure an auto-renewable subscription, you need to submit it to App Review for approval before it can be available to users.

### Submit a subscription

The first step in preparing an auto-renewable subscription for review is to upload a screenshot to App Review to show what the auto-renewable subscription looks like to users.

You accomplish this task by using the `/v1/subscriptionAppStoreReviewScreenshots` endpoint. This workflow is similar to the existing image workflows for App Clip images and app screenshots.

In the case of the auto-renewable subscription screenshot, you submit a single image using the following steps:

1.  Make an image reservation with `POST /v1/subscriptionAppStoreReviewScreenshots` (Create a Review Screenshot for an Auto-Renewable Subscription).

2.  Upload the image using the `PUT` URL provided in the response to the previous `POST`.

3.  After your image uploads, use `PATCH /v1/subscriptionAppStoreReviewScreenshots/{id}` (Commit a Review Screenshot for an Auto-Renewable Subscription) to commit the image.

4.  Finally, use `GET /v1/subscriptionAppStoreReviewScreenshots/{id}` (Read Subscription Review Screenshot Information) to confirm that the image is in place.

For more information, see Uploading Assets to App Store Connect.

Important

You need to submit your first subscription with an app binary submission. This must be done through appstoreconnect.apple.com. For subsequent subscriptions, you can submit using the following API endpoint without an associated app binary submission.

If this isn’t your first subscription, use `POST /v1/subscriptionSubmissions` (Create a Review Submission for a Subscription).

Here’s an example payload:

```
{
  "data": {
    "type": "subscriptionSubmissions",
    "relationships": {
      "subscription": {
        "data": {
          "type": "subscriptions",
          "id": "6446671421"
        }
      }
    }
  }
}
```

After you upload your screenshot for App Review, the next step is submission.

### Submit a subscription group

The localized metadata for a subscription group is submitted to App Review when a subscription within the subscription group is submitted. A subscription group can be submitted independently if you change localization metadata without changing a subscription. To submit a subscription group for review, use `POST /v1/subscriptionGroupSubmissions` (Create a Review Submission for a Subscription Group), where the `id` is that of the subscription group.

Here’s an example payload:

```
{
  "data": {
    "type": "subscriptionGroupSubmissions",
    "relationships": {
      "subscriptionGroup": {
        "data": {
          "id": "2000037020",
          "type": "subscriptionGroups"
        }
      }
    }
  }
}
```

## See Also

### Submitting Subscriptions and Groups for App Review

Subscription and Subscription Group Submissions

Create review submissions for auto-renewable subscriptions and subscription groups.


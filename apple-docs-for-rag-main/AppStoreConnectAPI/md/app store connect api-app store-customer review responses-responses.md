

- App Store Connect API
- App Store
-  Customer Review Responses 

API Collection

# Customer Review Responses

Get, create, update, and delete your responses to customer reviews.

## Overview

The `customerReviewResponses` resource represents your responses to customer reviews for apps you publish on the App Store. Each customer review can have at most one review response.

Use this API to get, create, update, and delete your responses to customer reviews for your app. First, get a list of customer reviews, including their resource IDs, by calling the List All Customer Reviews for an App or List All Customer Reviews for an App Store Version endpoints. Next use this API as follows:

- Respond to a customer review by calling Create or Update a Response to a Customer Review using the review’s resource ID. Update your existing review using the same endpoint.

- Get your existing review response by calling Get a Customer Review Response, using the resource ID of the customer review.

- Delete your response to a customer review by calling Delete a Response to a Customer Review, using the resource ID of your response.

For more information about reviews, see Ratings, Reviews, and Responses.

## Topics

### Getting Review Responses

Get a Customer Review Response

Get the response to a specific customer review.

Read Customer Review Response Information

Get information about a specific response you wrote to a customer review, including the response content and its state.

### Creating, Updating, and Deleting Review Responses

Create or Update a Response to a Customer Review

Create a response or replace an existing response you wrote to a customer review.

Delete a Response to a Customer Review

Delete a specific response you wrote to a customer review.

### Objects and Types

object CustomerReviewResponseV1Response

A response that contains a single Customer Review Responses resource.

object CustomerReviewResponseV1

The data structure that represents the Customer Review Responses resource.

object CustomerReviewResponseV1CreateRequest

The request body to use to create a response to a customer review.

object CustomerReview

The data structure that represents a Customer Reviews resource.

## See Also

### Customer Reviews and Responses

Customer Reviews

Get the customer reviews for your app.


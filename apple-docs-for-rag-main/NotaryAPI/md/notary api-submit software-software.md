

- Notary API
-  Submit Software 

Web Service Endpoint

# Submit Software

Start the process of uploading a new version of your software to the notary service.

Notary API 2.0.0+

## URL

``` source
POST https://appstoreconnect.apple.com/notary/v2/submissions
```

## HTTP Body

NewSubmissionRequest

Information about a new software submission that you want to make.

Content-Type: application/json

## Response Codes

` 200 ``OK`

NewSubmissionResponse

`OK`

The service recieved your submission request. The response includes information that you use to upload your software and track the status of your submission.

Content-Type: application/json

## Mentioned in 

Submitting software for notarization over the web

## Discussion

Use this endpoint to tell the notary service about a new software submission that you want to make. Do this when you want to notarize a new version of your software.

You provide an HTTP body that contains a name for the submission, a hash of the software that you plan to submit, and an optional webhook that the service uses to notify you when notarization completes. For the name, use the name of the file that you upload, including the `dmg` or `zip` extension. The service responds with temporary security credentials that you use to submit the software to Amazon S3 and a submission identifier that you use to track the submission’s status.

After uploading your software, you can use the identifier to ask the notary service for the status of your submission using the Get Submission Status endpoint. If you lose the identifier, you can get a list of your team’s 100 most recent submissions using the Get Previous Submissions endpoint. After notarization completes, use the Get Submission Log to get details about the outcome of notarization. Do this even if notarization succeeds, because the log might contain warnings that you can fix before your next submission.

### Example

- Request
- Response

```
{
  "notifications": [
    {
      "channel": "webhook",
      "target": "https://example.com"
    }
  ],
  "sha256": "68d561c564ef61f718e99a81b13bcb52af11b7ac9baf538af3ea0c83326fb6a1",
  "submissionName": "OvernightTextEditor_11.6.8.zip"
} 
```

```
{
  "data": {
    "attributes": {
      "awsAccessKeyId": "ASIAIOSFODNN7EXAMPLE",
      "awsSecretAccessKey": "wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY",
      "awsSessionToken": "AQoDYXdzEJr...",
      "bucket": "EXAMPLE-BUCKET",
      "object": "EXAMPLE-KEY-NAME"
    },
    "id": "2efe2717-52ef-43a5-96dc-0797e4ca1041",
    "type": "newSubmissions"
  },
  "meta": {
  }
} 
```

## See Also

### Software submission

object NewSubmissionRequest

Data that you provide when starting a submission to the notary service.

object NewSubmissionResponse

The notary service’s response to a software submission.


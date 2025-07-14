

- Vision
- Original Objective-C and Swift API
-  Recognizing Text in Images 

Article

# Recognizing Text in Images

Add text-recognition features to your app using the Vision framework.

## Overview

One of Vision’s many powerful features is its ability to detect and recognize multilanguage text in images. You can use this functionality in your own apps to handle both real-time and offline use cases. In all cases, all of Vision’s processing happens on the user’s device to enhance performance and user privacy.

Vision’s text-recognition capabilities operate using one of these paths:

Fast  
The fast path uses the framework’s character-detection capabilities to find individual characters, and then uses a small machine learning model to recognize individual characters and words. This approach is similar to traditional optical character recognition (OCR).

For example code using the fast path, see Extracting phone numbers from text in images.

Accurate  
The accurate path uses a neural network to find text in terms of strings and lines, and then performs further analysis to find individual words and sentences. This approach is much more in line with how humans read text.

For example code using the accurate path, see Structuring Recognized Text on a Document.

Using either path, you may optionally apply a language-correction phase based on Natural Language Processing (NLP) to minimize the potential for misreadings.

Note

Using Vision’s text-recognition features is similar to performing other Vision operations, where you perform computer vision requests on an image and retrieve the resulting observations. If you’re new to the Vision framework, see Detecting Objects in Still Images.

### Perform a Text-Recognition Request

Vision provides its text-recognition capabilities through VNRecognizeTextRequest, an image-based request type that finds and extracts text in images. The following example shows how to use VNImageRequestHandler to perform a VNRecognizeTextRequest for recognizing text in the specified CGImage.

```
// Get the CGImage on which to perform requests.
guard let cgImage = UIImage(named: "snapshot")?.cgImage else { return }

// Create a new image-request handler.
let requestHandler = VNImageRequestHandler(cgImage: cgImage)

// Create a new request to recognize text.
let request = VNRecognizeTextRequest(completionHandler: recognizeTextHandler)

do {
    // Perform the text-recognition request.
    try requestHandler.perform([request])
} catch {
    print("Unable to perform the requests: \(error).")
}
```

Note

VNRecognizeTextRequest uses the accurate path by default. To select the fast path, set the request’s recognitionLevel property to VNRequestTextRecognitionLevel.fast.

### Process the Results

After the request handler processes the request, it calls the request’s completion closure, passing it the request and any errors that occurred. Retrieve the observations by querying the request object for its results, which it returns as an array of VNRecognizedTextObservation objects. Each observation provides the recognized text string, along with a confidence score that indicates the confidence in the accuracy of the recognition.

```
func recognizeTextHandler(request: VNRequest, error: Error?) {
    guard let observations =
            request.results as? [VNRecognizedTextObservation] else {
        return
    }
    let recognizedStrings = observations.compactMap { observation in
        // Return the string of the top VNRecognizedText instance.
        return observation.topCandidates(1).first?.string
    }

    // Process the recognized strings.
    processResults(recognizedStrings)
}
```

If you’d like to render the bounding rectangles around recognized text in your user interface, you can also retrieve that information from the observation. The rectangles it provides are in normalized coordinates. To render them correctly in your user interface, convert CGRect instances from normalized coordinates to image coordinates by using the VNImageRectForNormalizedRect(_:_:_:) function as shown below.

```
let boundingRects: [CGRect] = observations.compactMap { observation in

    // Find the top observation.
    guard let candidate = observation.topCandidates(1).first else { return .zero }

    // Find the bounding-box observation for the string range.
    let stringRange = candidate.string.startIndex..

The resulting bounding box differs depending on the path you choose. The fast path calculates the recognized text’s bounding rectangle based on its individual characters. The accurate path tokenizes on whitespace, which means when working with Chinese text, the resulting bounding boxes will likely contain lines or line fragments instead of complete text.

### Optimize Language Settings

Your choice of fast or accurate path, along with your use of a particular API revision, determines the language support the text-recognition algorithms provide. To determine which languages a particular path and revision support, call the request’s supportedRecognitionLanguages(for:revision:) class method.

If not otherwise specified, Vision biases its results toward English. To alter its default behavior, provide an array of supported languages in the request’s recognitionLanguages property. The order in which you provide the languages dictates their relative importance. To recognize traditional and simplified Chinese, specify `zh-Hant` and `zh-Hans` as the first elements in the request’s recognitionLanguages property. English is the only other language that you can pair with Chinese.

Enabling language correction on the request helps minimize common recognition errors. If the text you’re recognizing uses domain-specific jargon, such as medical or technical terms, you can tailor the language correction’s behavior by setting the request’s customWords property. Language correction gives precedence to the custom words when performing its processing. The request ignores the customWords property if language correction isn’t enabled.

Note

Vision doesn’t support language correction, or its related customWords array, for Chinese.

## See Also

### Text recognition

Structuring Recognized Text on a Document

Detect, recognize, and structure text on a business card or receipt using Vision and VisionKit.

Extracting phone numbers from text in images

Analyze and filter phone numbers from text in live capture by using Vision.

Locating and displaying recognized text

Perform text recognition on a photo using the Vision framework’s text-recognition request.

class VNRecognizeTextRequest

An image-analysis request that finds and recognizes text in an image.

class VNRecognizedTextObservation

A request that detects and recognizes regions of text in an image.




- TVMLKit JS
- Slideshow
-  append 

Instance Method

# append

Add additional images to a currently running slideshow.

tvOS 10.0+

``` source
void append(
    in Object imageRequests
);
```

## Parameters 

`imageRequests`  

An array of image request objects.

## Discussion

The `imageRequests` parameter contains an array of image request objects that can have the following formatting:

- An array of URLs.

- A dictionary with two key-value pairs, `headers` and `urls`. `headers` provides a dictionary of headers that is included with all image requests. `urls` contains an array of URLs.

## See Also

### Creating and Modifying a Slideshow

dismiss

Dismisses a currently running slideshow.

start

Starts a slideshow with the given set of images.


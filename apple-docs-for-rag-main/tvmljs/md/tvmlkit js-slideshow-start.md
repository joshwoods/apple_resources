

- TVMLKit JS
- Slideshow
-  start 

Instance Method

# start

Starts a slideshow with the given set of images.

tvOS 10.0+

``` source
void start(
    in Object imageRequests, 
    in Object options, 
    in Function exitCB
);
```

## Parameters 

`imageRequests`  

An array of image request objects.

`options`  

An optional set of options that modify the slideshow. If no options are specified, a default of `false` or `0`is used.

`exitCB`  

An optional callback function that is called when the slideshow is dismissed. If this parameter is not specified, the page on top of the navigation stack is displayed.

## Discussion

When a new slideshow beings using the `start` function, if there is a currently running slideshow, that slideshow is dismissed. The `imageRequests` parameter contains an array of image request objects that can have the following formatting:

- An array of URLs.

- A dictionary with two key-value pairs, `headers` and `urls`. `headers` provides a dictionary of headers that is included with all image requests. `urls` contains an array of URLs.

If the `showSettings` key in the `options` parameter is set to `true` or `1`, the user will be asked to pick a theme before the slideshow begins. Listing 1 shows an example of a simple slideshow that is created with two images.

function mySlideshow() {
   var images = [&#39;path to image&#39;, &#39;path to image&#39;];
   Slideshow.start(images, { &#39;showSettings&#39;: &#39;0&#39; });
}

Listing 1 Creating a new slideshow example

## See Also

### Creating and Modifying a Slideshow

append

Add additional images to a currently running slideshow.

dismiss

Dismisses a currently running slideshow.


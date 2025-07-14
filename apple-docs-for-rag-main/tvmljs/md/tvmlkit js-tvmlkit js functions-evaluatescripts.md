

- TVMLKit JS
- TVMLKit JS Functions
-  evaluateScripts 

Function

# evaluateScripts

Verifies and executes TVMLKit JS files.

tvOS 9.0+

``` source
void evaluateScripts(
    in Array scripts, 
    in Function callback
);
```

## Parameters 

`scripts`  

An array of URLs pointing to TVMLKit JS files.

`callback`  

A function that is executed after attempting to open the TVMLKit JS files. A boolean argument is passed into the function that signals whether all scripts loaded successfully.

## Discussion

This method first verifies that the locations contained in the `scripts` parameter contain TVMLKit JS files. The code in the files is then executed. The callback function contains a boolean argument that signals whether the TVMLKit JS files loaded successfully. Use this method to keep the size of your initial TVMLKit JS file small, while being able to incorporate other TVMLKit JS files. Listing 1 shows an example incorporating this method into your app. The example creates an array containing the location of the ResourceLoader and Presenter TVMLKit JS files. On a successful load, the `success` parameter is set to `TRUE` and the app continues. Otherwise, an alert is presented onscreen stating that an error occurred.

App.onLaunch = function(options) {
    var javascriptFiles = [
        `${options.BASEURL}js/ResourceLoader.js`,
        `${options.BASEURL}js/Presenter.js`
    ];

    evaluateScripts(javascriptFiles, function(success) {
        if (success) {
            resourceLoader = new ResourceLoader(options.BASEURL);

            var index = resourceLoader.loadResource(`${options.BASEURL}templates/Index.xml.js`,
                function(resource) {
                    var doc = Presenter.makeDocument(resource);
                    doc.addEventListener(&quot;select&quot;, Presenter.load.bind(Presenter));
                    navigationDocument.pushDocument(doc);
                });
        } else {

            var alert = createAlert(&quot;Evaluate Scripts Error&quot;, &quot;There was an error attempting to evaluate the external JavaScript files.\n\n Please check your network connection and try again later.&quot;);
            navigationDocument.presentModal(alert);

            throw (&quot;Playback Example: unable to evaluate scripts.&quot;);
        }
    });
}

Listing 1 evaluateScripts example


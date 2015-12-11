In order to add a map to a page you need to create an html element you can target with jQuery and include the map compare JS & CSS files. Once the element exists in the DOM you can add a map by targetting it with jQuery and calling the `mapCompare` jQuery function created by the map compare JS file.
The `mapCompare` function takes an object as its parameter. This object needs one key, `config` which points to either a string or another object. If it points to a string then the string needs to be a reference to a json config file. If security requirements won't let you host flat files then you can use a javascript object -- which just needs to be the contents of the existing config files.

``` javascript
$('#EXAMPLE-SELECTOR').mapCompare({config: 'CONFIG-FILE.json'});
```
## Welcome to nicecountryinput

An easy-to-use country picker.

### Dependencies and requirements

- Javascript, CSS
- jQuery 2.x / 3.x
- HTML data-* Attributes
- Base64 img source support

### Features

- English and Native country name
- Selected country is set by ISO code
- Additional selectors for Continents
- Additional selectors for All / None
- Filter input (works with native and english country name)
- No global namespace pollution, everything is in one prototype "NiceCountryInput"
- No image files (Every image is saved in the JS file)

### Usage

- Include niceCountryInput.css and niceCountryInput.js

```html
 <div id="testinput" style="width: 300px;" data-selectedcountry="US" data-showspecial="false" data-showflags="true" 
   data-i18nall="All selected" data-i18nnofilter="No selection" data-i18nfilter="Filter" data-onchangecallback="onChangeCallback" />
 </div>

 <script>
    function onChangeCallback(ctr){
        console.log("The country was changed: " + ctr);
    }
    $(document).ready(function () {
        new NiceCountryInput($("#testinput")).init();
    });
 </script>
 
```
 
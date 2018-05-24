## Welcome to nicecountryinput

An easy-to-use country picker. Just 1 JS and 1 CSS file.

<a href="https://masbaehr.github.io/nicecountryinput/" target="_blank">Show Demo!</a>

Usage: 

```html

    <script src="niceCountryInput.js"></script>
    <link rel="stylesheet" type="text/css" href="niceCountryInput.css">

    <div id="testinput" style="width: 300px;" data-selectedcountry="US" data-showspecial="false"
        data-showflags="true" data-i18nall="All selected" data-i18nnofilter="No selection" 
        data-i18nfilter="Filter" data-onchangecallback="onChangeCallback" />
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
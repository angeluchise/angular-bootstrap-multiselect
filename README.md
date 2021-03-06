angular-bootstrap-multiselect
==========================

A multiselect dropdown list for AngularJS styled to fit the Twitter Bootstrap standard design

Screenshot:

![Screenshot](/multiselect.png?raw=true "Screenshot")

Originally created by Amitava Saha (https://github.com/amitava82/angular-multiselect)

Modified by Sebastian Hammerl (https://github.com/sebastianha/angular-bootstrap-multiselect)



### Installation via Bower:

```
$ bower install angeluchise-angular-bootstrap-multiselect --save
```

### Usage:

Add "ui.multiselect" to your modules list. Then you can use it like follows:

```
<multiselect
    ng-model="selectModel"
    options="c for c in selectOptions"    // use ... c.name for c in ... for objects
    data-multiple="true"                  // true for multi-select mode
    data-compare-by="id"                  // set key to compare objects, otherwise is has to be equal to options
    data-header-key="header"              // Key which marks headers in the objects list
    data-divider-key="divider"            // Key which marks dividers in the objects list
    scroll-after-rows="5"                 // Show scroll bar after 5 rows
    filter-after-rows="5                  // Show filter input after 5 rows
    max-width="100"                       // The maximum width of the multiselect dropdown button
    ms-header="select"                    // The name of the multiselect
    ms-search="Filter by name"            // the text of the input of search
    ms-selecteds="Selecteds"              // the text of the header selecting the items
    tabindex="-1">                        // tabindex setting for dropdown
</multiselect>
```

See index.html and app.js for examples and how it works.

### Testing:

Start web server e.g. via Python:
```
$ python -m SimpleHTTPServer 8000
```

Start Karma E2E tests (has to be installed globally before):
```
$ karma start
```

### License
Copyright (c) 2018 Angel Perez

Copyright (c) 2017 Sebastian Hammerl, Getslash GmbH

Copyright (c) 2014 Amitava Saha

Licensed under the MIT License

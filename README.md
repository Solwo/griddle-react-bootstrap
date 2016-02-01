# Griddle Bootstrap

- [About](#about)
- [Quick Start](#quick-start)
- [License](#license)

## About

[Bootstrap](http://getbootstrap.com/) style for [react-griddle](http://griddlegriddle.github.io/Griddle/).

Features:

* Bootstrap style [Custom Paging Component of Griddle](http://griddlegriddle.github.io/Griddle/customization.html).
* Preconfigured Griddle Component.

## Quick Start

Install this library and the dependencies by npm.

```bash
npm install griddle-react-bootstrap --save
npm install react react-dom --save
npm install griddle-react --save
npm install react-bootstrap --save
```

And import and render component you want to use. Please check [example page](http://wadahiro.github.io/griddle-react-bootstrap/).

```js
import { BootstrapPager, GriddleBootstrap } from 'griddle-react-bootstrap';

...

    <Griddle
        tableClassName={'table table-bordered table-striped table-hover'}
        useGriddleStyles={false}
        results={fakeData}
        showSettings={true}
        showFilter={true}
        useCustomPagerComponent={true}
        customPagerComponent={ BootstrapPager }
        />

or

    <GriddleBootstrap bordered={true} hover={true} striped={true} results={fakeData} />
```

And import custom css for griddle (`griddle-react-bootstrap.css`) which is included in `node_modules/griddle-react-bootstrap/dist` directory.

## License

Licensed under the [MIT](/LICENSE.txt) license.
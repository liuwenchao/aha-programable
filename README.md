# &lt;aha-programable&gt;

> A custom element to calculate a piece of js code and use the result as the content.
> This helps when you don't want to start a script block or a new javascript file.

## Demo

[Check it live!](http://liuwenchao.github.io/aha-programable)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install aha-programable --save
```

Or [download as ZIP](https://github.com/liuwenchao/aha-programable/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/platform/platform.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/aha-programable/dist/aha-programable.html">
    ```

3. Start using it!

    ```html
    <aha-programable></aha-programable>
    ```

## Options

Attribute     | Options     | Default      | Example | Description
---           | ---         | ---          | ---     | ---
`value`       | *string*    | ``           | var today = new Date(); return today.toISOString(); | You can provide any js code here, just remember to add a return on the final result.

## Methods

Method        | Parameters   | Returns     | Description
---           | ---          | ---         | ---

## Events

Event         | Description
---           | ---

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

* To build the distribution files before releasing a new version.

    ```sh
    $ grunt build
    ```

* To provide a live demo, send everything to `gh-pages` branch.

    ```sh
    $ grunt deploy
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

For detailed changelog, check [Releases](https://github.com/liuwenchao/aha-programable/releases).

## License

[MIT License](http://opensource.org/licenses/MIT)

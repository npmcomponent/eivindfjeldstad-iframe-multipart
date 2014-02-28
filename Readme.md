*This repository is a mirror of the [component](http://component.io) module [eivindfjeldstad/iframe-multipart](http://github.com/eivindfjeldstad/iframe-multipart). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/eivindfjeldstad-iframe-multipart`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# iframe-multipart

  Multipart transport for old browsers.
  A minmal port of [jQuery-File-Upload](https://github.com/blueimp/jQuery-File-Upload), without the jQuery part.

## Installation

  Install with [component(1)](http://component.io):

    $ component install eivindfjeldstad/iframe-multipart

## Example
```js
var submit = require('iframe-multipart');
var form = document.getElementById('some-multipart-form');

submit(form, function (err, res) {
  // all done
});
```

## Gotchas
The response type should always be ```text/html```. See the `example` folder.
If you are responding with user generated content you should probably wrap it in a `<textarea>` for security reasons.

## API
### submit(form, fn)
Submits `form` and calls `fn` when done.

## License

  MIT

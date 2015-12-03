# protocols [![Support this project][donate-now]][paypal-donations]

Get the protocols of an input url.

## Installation

```sh
$ npm i --save protocols
```

## Example

```js
// Dependencies
var Protocols = require("protocols");

console.log(Protocols("git+ssh://git@some-host.com/and-the-path/name"));
// => ["git", "ssh"]

console.log(Protocols("http://ionicabizau.net", true));
// => "http"
```

## Documentation

### `Protocols(input, first)`
Returns the protocols of an input url.

#### Params
- **String** `input`: The input url.
- **Boolean|Number** `first`: If `true`, the first protocol will be returned. If number, it will represent the zero-based index of the protocols array.

#### Return
- **Array|String** The array of protocols or the specified protocol.

## How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].

## Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:

 - [`is-ssh`](https://github.com/IonicaBizau/node-is-ssh)

 - [`parse-url`](https://github.com/IonicaBizau/node-parse-url)

## License

[MIT][license] © [Ionică Bizău][website]

[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(http%3A%2F%2Fionicabizau.net)&year=2015#license-mit
[website]: http://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
_My Gravatar demo projects are for users to get acquainted with languages and platforms with something more than a "Hello World" example. Versions are available for [Clojure](https://brackendev.github.io/GravatarDemo-Clojure/), [F#](https://brackendev.github.io/GravatarDemo-FSharp/), [Newspeak](https://brackendev.github.io/GravatarDemo-Newspeak/), [Pharo](https://brackendev.github.io/GravatarDemo-Pharo/), and [Squeak](https://brackendev.github.io/GravatarDemo-Squeak/)._

- - -

GravatarDemo-Pharo
==================

**[Pharo](https://www.pharo.org/) implementation to interact with the [Gravatar API](https://en.gravatar.com/site/implement/).**

* [Pharo 7](https://www.pharo.org/) reference platform.
* Examples and tests included.

## Installation

In a Playground, evaluate:

```smalltalk
Metacello new 
  repository: 'github://brackendev/GravatarDemo-Pharo';
  baseline: 'Gravatar';
  load.
```

## Example Usage

In a Playground, evaluate:

```smalltalk
Gravatar exampleRetrieveImageForEmail.
```

```smalltalk
Gravatar exampleRetrieveImageForEmailSizeRating.
```

```smalltalk
Gravatar exampleRetrieveProfileForEmail.
```

```smalltalk
"Retrieve the image for the email address, open in an inspector"
(Gravatar retrieveImageForEmail: 'email@example.com') inspect.
```

```smalltalk
"Retrieve the image (200 px by 200 px, rated 'G' or 'PG') for the email address, open in an inspector"
(Gravatar retrieveImageForEmail: 'email@example.com' size: 200 rating: 'pg') inspect.
```

```smalltalk
"Retrieve the profile for the email address, open in an inspector"
(Gravatar retrieveProfileForEmail: 'email@example.com') inspect.
```

## Acknowledgements

This project makes use of the following third-party libraries:

* [NeoJSON](https://github.com/svenvc/NeoJSON)
* [Zinc HTTP Components](https://github.com/svenvc/zinc)

## Author

[brackendev](https://www.github.com/brackendev)

## License

GravatarDemo-Pharo is released under the MIT license. See the LICENSE file for more info.

- - -

## Useful Links

* [@pharoproject](https://twitter.com/pharoproject) [Twitter]
* [forum.world.st](http://forum.world.st/)
* [pharo.org](http://www.pharo.org/)

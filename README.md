# Compass Normalize.css

This simple plugin for [Compass](http://compass-style.org/) enables you to use [normalize.css](http://necolas.github.com/normalize.css/) in your stylesheets without having to download it.


## Installation

From the command line:

```
$ (sudo) gem install compass-normalize
```

You can also install the gem from your local fork:

```
$ git clone git://github.com/ksmandersen/compass-normalize.git
$ rake build
$ rake install
```
	
## Normalize Versions
Normalize has two versions, a modern Normalize for Firefox 4+, Chrome, Safari 5+, Opera, and Internet Explorer 8+, and a legacy Normalize with support for all legacy versions of those browsers.

## Usage

### Modern Normalize
When creating a new project with compass:

```
$ compass create <my_project> -r compass-normalize --using compass-normalize
```

If using an existing project, edit your config.rb and add this line:

```ruby
require 'compass-normalize'
```

To use the normalize plugin, just import and include normalize:

```scss
@import normalize;
```

You can also just import parts you need:

```scss
@import 'normalize/html5';
@import 'normalize/base';
@import 'normalize/links';
@import 'normalize/typography';
@import 'normalize/embeds';
@import 'normalize/figures';
@import 'normalize/forms';
@import 'normalize/tables';
```

### Legacy Normalize
When creating a new project with compass:

```
$ compass create <my_project> -r compass-normalize --using compass-normalize/legacy
```

If using an existing project, edit your config.rb and add this line:

```ruby
require 'compass-normalize'
```

To use the normalize plugin, just import and include normalize:

```scss
@import normalize-legacy;
```

You can also just import parts you need:

```scss
@import 'normalize-legacy/html5';
@import 'normalize-legacy/base';
@import 'normalize-legacy/links';
@import 'normalize-legacy/typography';
@import 'normalize-legacy/lists';
@import 'normalize-legacy/embeds';
@import 'normalize-legacy/figures';
@import 'normalize-legacy/forms';
@import 'normalize-legacy/tables';
```

## Acknowledgements
Many thanks to [Frederic Hemberger](https://github.com/fhemberger/) and [Sam Richard](https://github.com/snugug) who contributed greatly to this project.

## License
This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to [The Unlicense](http://unlicense.org/)

### Major components:

* [normalize.css](http://necolas.github.com/normalize.css/): Public domain
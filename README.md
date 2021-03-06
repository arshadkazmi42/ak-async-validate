# URL Validate

[![Build Status](https://travis-ci.org/arshadkazmi42/ak-url-validate.svg?branch=master)](https://travis-ci.org/arshadkazmi42/ak-url-validate)
[![NPM Downloads](https://img.shields.io/npm/dt/ak-url-validate.svg)](https://www.npmjs.com/package/ak-url-validate)
[![Package Size](https://img.shields.io/bundlephobia/min/ak-url-validate.svg)](https://www.npmjs.com/package/ak-url-validate)
[![NPM Version](https://img.shields.io/npm/v/ak-url-validate.svg)](https://www.npmjs.com/package/ak-url-validate)
[![Contributors](https://img.shields.io/github/contributors/arshadkazmi42/ak-url-validate.svg)](https://github.com/arshadkazmi42/ak-url-validate/graphs/contributors)
[![Commit](https://img.shields.io/github/last-commit/arshadkazmi42/ak-url-validate.svg)](https://github.com/arshadkazmi42/ak-url-validate/commits/master)

This library helps in validating whether a url exists or not. It verifies url pattern and whether the url is up and running.

<a href="https://www.buymeacoffee.com/arshadkazmi42" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
<a href="https://www.patreon.com/bePatron?u=15454240" target="_blank"><img src="https://c5.patreon.com/external/logo/become_a_patron_button.png" alt="Become a Patron!" height="39"></a>

Please consider donating, if you like my work


## Install
```
npm install ak-url-validate
```

## Usage

```js
var auv = require('ak-url-validate');

const url = 'http://github.com/arshadkazmi42';
const response = await auv.isValidUrl(url);
if (response.isValid) {
  // Do something if the url is valid
} else {
  // Do something if url is invalid
}

```

## Status Codes
isValid function returns status code whatever is returned from the url response. Some of the status codes are mentioned below

- **SUCCESS**: This code is returned when the url is up and running.

```
{
  code: "SUCCESS",
  isValid: true
}
```

- **404**: This code is returned when the url is not found. 

```
{
  code: 404,
  isValid: false,
  message: "Not Found"
}
```

- **ETIMEDOUT**: This code is returned when the url is not responsding and get timed out.

```
{ 
  isValid: false, 
  code: "ETIMEDOUT",
  message: "Invalid Url" 
}
```

- **INVALID**: This is an exception code, if the url does not return any status code, this code is returned in the response

```
{
  isValid: false, 
  code: "INVALID",
  message: "Invalid Url" 
}
```

## Contributing Guidelines

Read the contributing guidelines [here](CONTRIBUTING.md)

## Contributors

[![](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/images/0)](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/links/0)[![](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/images/1)](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/links/1)[![](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/images/2)](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/links/2)[![](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/images/3)](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/links/3)[![](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/images/4)](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/links/4)[![](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/images/5)](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/links/5)[![](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/images/6)](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/links/6)[![](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/images/7)](https://sourcerer.io/fame/arshadkazmi42/arshadkazmi42/ak-url-valdiate/links/7)

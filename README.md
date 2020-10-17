# validlist
Basic Array-based validation module

# Usage
You can provide the module with an array of values. If one of the given values counts as negative (false, null, undefined, etc), false will be returned.

# Example
In this example plain types are such as booleans, strings and more are being used, but you could of course fill an array with responses from functions afterwhich they can all be validated at once.

```javascript
    const validate = require('validlist');
    const validation1 = [true, 1, 'string'];
    const validation2 = [true, 1, 'string', null];

    validate(validation1);      //true, no negative values.
    validate(validation2);      //false, contains null which counts as negative.
```

# Contribution
Please make a pull request. For major changes i kindly ask you to create an issue first where in you can discuss your changes.

# Licence
[MPL-2.0](https://www.mozilla.org/en-US/MPL/2.0/)
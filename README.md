# Uri query parameters extracter for JavaScript
A simple url parser in JavaScript

1. Allows you to parse a url in conformance to WHATWG specs
2. Allows you to extract query search parameter values
3. Works for url with multiple parameters

# Example usage

```ts
import { Parser } from 'uri-param-parser'
let parser = new Parser('http://example.com/?name=danny-sofftie')
// parses a url in accordance to WHATWG uri specs
let paramValue = parser.extract()
// will return an object as { param: value }
```
# Pass search parameter 
```ts
let paramValue = parser.extract('name')
// will return 'value' of the parameter passed
// e.g. 'danny-sofftie'
```
# License
MIT License contributions are welcome

```
Copyright Danny Sofftie <dankim761@gmail.com>. All rights reserved

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to
deal in the Software without restriction, including without limitation the
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
sell copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
IN THE SOFTWARE.
```
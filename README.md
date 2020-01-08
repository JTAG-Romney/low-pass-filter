# low-pass-filter 

A low pass filter.

## Install
```
npm install low-pass-filter
```

## Use

### Browser
Use the **low-pass-filter.js** file in the */dist* folder:
```html
<script src="./dist/low-pass-filter.js"></script>
<script>
lowPassFilter.lowPassFilter(samples, 22050, 44100, 2);
</script>
```

Or load it from the [jsDelivr](https://cdn.jsdelivr.net/npm/low-pass-filter) CDN:
```html
<script src="https://cdn.jsdelivr.net/npm/low-pass-filter"></script>
```

Or load it from [unpkg](https://unpkg.com/low-pass-filter):
```html
<script src="https://unpkg.com/low-pass-filter"></script>
```

### Node
```javascript
const lowPassFilter = require('low-pass-filter').lowPassFilter;
lowPassFilter(samples, 22050, 44100, 2);
```

## API
```javascript

/**
 * Low pass filter.
 * @param {!Array<number>|TypedArray} samples The samples.
 * @param {number} cutoff The cutoff frequency.
 * @param {number} sampleRate The sample rate.
 * @param {number} numChannels The number of channels.
 */
function lowPassFilter(samples, cutoff, sampleRate, numChannels) {}
```

### References
https://github.com/jiaaro/pydub/blob/master/pydub/effects.py#L187  
http://stackoverflow.com/questions/13882038/implementing-simple-high-and-low-pass-filters-in-c

## LICENSE
Copyright (c) 2018 Rafael da Silva Rocha.  
Copyright (c) 2011 James Robert, http://jiaaro.com

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

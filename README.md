# bitter
Bit-Depth Reduction

This module reduces the bit-depth of the input signal
Check out this article on Wikipedia about bit-depth in audio: 
https://en.wikipedia.org/wiki/Audio_bit_depth
   
For n bit-depth, we have 2^n possible values for a sample.
For example, if the bit-depth is 8, we have 256 possible values ranging from -128 to 127.

## Usage
```javascript
import Bitter from 'opendsp/bitter';

export function dsp(t) {
  var input = ... ;

  return Bitter(4).setPreGain(4).setPostGain(0.25).run( input );
  // 4-bit sample depth.
}
```
  
  

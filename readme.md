#iago

encode ogg in the browser

- something odd about ScriptProcessorNode in chrome right now, but firefox is working fine.

###Credit where credit is due

- Thanks to halfvector for the heavy work on this:
  - http://hotcashew.com/2014/02/chrome-audio-api-and-ogg-vorbis/
  - https://gist.github.com/halfvector/9105335
- Thanks to devongovett for the ogg.js repo
  - https://github.com/devongovett/ogg.js
- Thanks to shovon for moving ogg.js forward and improved documentation
  - https://github.com/shovon/libvorbis.js

###Usage

```javascript

// stream is 
var iago = new Iago( stream );

// Do your stream thing

// Get your compressed ogg
iago.getBlob( function( err, blob ) {
  // blob is of type audio/ogg
});
```

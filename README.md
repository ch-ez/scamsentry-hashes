# normal users
public bot:
https://ch-ez.github.io/ScamSentry-site/

# developers:
## how to use the hash list for your own projects

use this for your app  
https://raw.githubusercontent.com/ch-ez/scamsentry-hashes/main/hashes.json

generate a perceptual hash for images  

https://en.wikipedia.org/wiki/Perceptual_hashing

DCT-based perceptual hash

64 character hash

node js phash 


```javascript
// node js phash
const fs = require("fs");
const phash = require("sharp-phash");

async function hashImage(path) {
  const buffer = fs.readFileSync(path);
  const hash = await phash(buffer);

  console.log(hash);
}

hashImage("image.png");
```


compare the hash against the list here

64-character binary hashes, compare using Hamming distance.  
If the distance is less than or equal to 12, treat it as a almost identical image.

this list gets updated super often, mainly targetting mrbeast scam campaign.

**very skidded**, but useful

example of hashed images in this json

<img width="716" height="428" alt="image" src="https://github.com/user-attachments/assets/0faa8f00-81c6-4639-9415-6898e6a9d558" />

<img width="716" height="428" alt="image" src="https://github.com/user-attachments/assets/890e155e-c549-4ed3-aab0-21d6bc689353" />

<img width="712" height="420" alt="image" src="https://github.com/user-attachments/assets/a4f77ef0-79df-401f-bdfc-018f9fa8aacd" />

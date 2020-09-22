# Exploring and experimenting with Javascript Minifier API

* Official Website - https://javascript-minifier.com/
* API Docs url - https://javascript-minifier.com/api/ 
* You can minify files directly from their website but I am gonna use their API to minify blackboard.js present in this repo. 

### Commands for minifing javascript files (according to official Website) - 

##### wget - 
```
wget --post-data='input=console.log( 1 );' --output-document=- https://javascript-minifier.com/raw

wget --post-data="input=`cat main.js`" --output-document=main.min.js https://javascript-minifier.com/raw
```

##### curl (which I'm gonna use) - 
```
curl -X POST -s --data-urlencode 'input=console.log( 1 );' https://javascript-minifier.com/raw

curl -X POST -s --data-urlencode 'input@main.js' https://javascript-minifier.com/raw > main.min.js
```

##### POST - 
```
POST https://javascript-minifier.com/raw?input=...
```

### Commands which I used - 
```
<!-- commands here -->
```
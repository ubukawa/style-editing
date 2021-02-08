# style-editing
working space for style editing.  
Based on "un-vector-tile-toolkit/onyx" and "unvt/naru."


# hosting at localhost
```zsh
git clone https://github.com/ubukawa/style-editing  
cd style-editing  
```  
Edit the config settings (tile location, etc).  
You can also add vector tiles (pbf or mbtiles)
pbf should be adde under htdocs. mbtiles should be added under mbtiles. (see app.js)  

```zsh
node app.js   
```

# hosting at local host (with Docker)
```zsh
git clone https://github.com/ubukawa/style-editing  
cd style-editing  
```  
Edit the config settings (tile location, etc).  
```zsh 
docker run -it --rm -v ${PWD}:/data -p 8836:8836 unvt/nanban
cd /data
node app.js  
```  

(make a style.json at Docker)
```zsh
rake
``` 


# map check
At localhost:  
http://localhost:8836/index.html

At maputnik:  
https://maputnik.github.io/editor/?style=http://localhost:8836/style.json

# refereneces  
onyx:
naru:


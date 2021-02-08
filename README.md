# hase-nanban
A developer friendly UNVT Dockerfile based on Ubuntu/Intel.  
unvt/nanban was slightly modified so that it runs hasekura


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
(check if server runs at http://localhost:8836/hello.html)


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


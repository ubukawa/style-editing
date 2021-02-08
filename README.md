# hase-nanban
A developer friendly UNVT Dockerfile based on Ubuntu/Intel.  
unvt/nanban was slightly modified so that it runs hasekura


# hosting at localhost
```zsh
git clone https://github.com/ubukawa/style-editing  
cd style-editing  
```  
Edit the config settings (tile location, etc).  

```zsh
node app.js   
```


# use
```zsh
docker rmi hase-nanban  
git clone https://github.com/ubukawa/hase-nanban  
cd hase-nanban  
docker build -t hase-nanban .  
docker run -it --rm -v ${PWD}:/data -p 8836:8836 hase-nanban  

```


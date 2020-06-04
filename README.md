# create-gcloud-function
Basic template to create google cloud function

## Npm scripts

### npm run watch
Start watching ts files in ./src, to automatically compile to ./build

### npm run start
Start function locally

### npm run deploy
Deploy to gcp cloud

I recommend creating the following script inside /usr/local/bin/create-gcloud-function

```
#!/bin/bash
git clone git@github.com:Tobjoern/create-gcloud-function.git $1
cd ./$1

#remove git repository
rm -rf ./.git

#remove README.md
unlink README.md

npm i

code .
```
This way you can call create-gcloud-function <name>, from everywhere to jumpstart your development!

Regards

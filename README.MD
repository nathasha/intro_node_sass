Source: 
https://medium.com/@brianhan/watch-compile-your-sass-with-npm-9ba2b878415b#.slc9j4h8h

## Install Dependencies
    npm install -D node-sass nodemon
    
-D flag is another way of saying “write these node_modules into my package.json under devDependencies” 

node-sass wraps Libsass.

nodemon will watch for changes on Sass files

## To have separate files for npm scripts

Move the files to bin folder without extension

Need to make the files in the bin folder executable

    chmod +x bin/build-css
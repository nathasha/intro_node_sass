Source: 
https://medium.com/@brianhan/watch-compile-your-sass-with-npm-9ba2b878415b#.slc9j4h8h

## Install Dependencies
    npm install -D node-sass nodemon
    
-D flag is another way of saying “write these node_modules into 
package.json under devDependencies” 

node-sass wraps Libsass.

## To Watch Sass Filles
    node-sass - w <sass__watch_dir>
    
   or 

    nodemon -e scss -x \”npm run build-css\”

nodemon : nodemon will watch the files in the directory in which nodemon was started, 
and if any files change, nodemon will automatically restart the node application.
In this case, it will watch for changes on Sass files

## To have separate files for npm scripts

Move the files to bin folder without extension

Need to make the files in the bin folder executable

    chmod +x bin/build-css
To run typescript on node we make use of the npm libraries typescript and ts-node installed locally
npm install -g typescript ts-node

to compile the typescript into JS code run the following command
tsc index.ts

we need to create a tsconfig.json file to customise the compiler, run this following command
tsc --init

in the file tsconfig.json change the following fields to indicate de source code and the build directory target:
"outDir": "./build",
"rootDirs": ["./src"],

use tsc -w to watch for changes and complie the code
tsc -w

we install nodemon and concurrently to automate the compiling and bulding of the application
nodemon to re-run the app everytime there are changes and concurrency to run 2 scripts at once.
npm install nodemon concurrently

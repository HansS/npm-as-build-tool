##Npm as a build tool
###Npm Commands
##Minimal Package File required fields:
```json
{
  name: "mypackage", // name with maximal 214 url-safe characters
  version: 0.0.1	
}
```
Name and version together mypackage@0.0.1 build the form an identifier that is assumed to be completley
unique.
###Npm package.json file
With the help of the scripts tag in the package.json file npm can be used to
run node code.
###Package.json Scripts Property
The "scripts" property is a dictionary containing script commands that are
run at various times in the lifecycle of your package. The key is the lifecycle event, and the value is 
the command to run at that point.
```json
{
	"name":"mypackage",
	"version":0.0.1,
	"scripts":{
		"test":"mocha"
	}
}
```
###Run a npm script entry
default script entry test and start can be run without 'run' command
npm test (short: npm t)
npm start
other script entries must be run with 'run':
npm run 'script entry'


Command | Description
--------|-------------
npm init -y | create a package.json with default values
npm t | run test script defined in package.json
npm run test | run a a script which is not test
npm i mocha --save-dev | install a dev library
ls node_modules/.bin   | show available npm commands




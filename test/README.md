## CaptAgent CI

Automated tests for Captagent using Node JS and Mocha.

NOTICE: `sudo` rights are required to spawn the agent and test sockets on interface `any`

### Usage
```
npm install -g mocha
sudo npm test
```

#### Units
##### Initialization
This suite will initialized the compiled agent and check it returns a version number.
```
sudo mocha init.js
```
##### HEP Functionality
This suite will test SIP and HEP features using the compiled agent, feeding it SIP and expecting HEP back.
```
sudo mocha hep.js
```
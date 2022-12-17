# koyeb-api-client
- An Unofficial koyeb-client (V0.0.1) to ease intraction with koyeb.com using asyncronous functions currently support one application.

## Installation
```js
npm install koyeb-api-client
```

## Usage/Examples

### 1. Redeploy
```js
//Redeploy koyeb service
const { redeploy } = require('koyeb-api-client');
let data = await redeploy(service_id,koyeb_api)
console.log(data)
```
### 2. Change Env Vars
```js
//change var from koyeb
const { change_env } = require('koyeb-api-client');
var env = 'x:y'
let data = await change_env(env,koyeb_api)
console.log(data)
```
### 3. Delete Env Var
```js
//Delete any var from koyeb
const { change_env } = require('koyeb-api-client');
var env = 'x'
let data = await delvar(env,koyeb_api)
console.log(data)
```
### 4. Get deployments
```js
//Get list of active deployments.
const { get_deployments } = require('koyeb-api-client');
let data = await get_deployments(koyeb_api)
console.log(data)
```
### 5. Get all koyeb vars
```js
const { getallvar } = require('koyeb-api-client');
let data = await getallvar(koyeb_api)
console.log(data)
```
### 6. Get single specific koyeb var
```js
const { getvar } = require('koyeb-api-client');
var key = 'x'
let data = await getvar(key,koyeb_api)
console.log(data)
```
### 7. Get services
```js
const { services } = require('koyeb-api-client');
let data = await services(koyeb_api)
console.log(data)
```

### 8. Delete services
```js
const { del_service } = require('koyeb-api-client');
let data = await del_service(service_id,koyeb_api)
console.log(data)
```

### 9. Pause service
```js
const { pause_service } = require('koyeb-api-client');
let data = await pause_service(service_id,koyeb_api)
console.log(data)
```
### 10. Resume service
```js
const { resume_service } = require('koyeb-api-client');
let data = await resume_service(service_id,koyeb_api)
console.log(data)
```
### 11. List services
```js
const { list_services } = require('koyeb-api-client');
let data = await list_services(koyeb_api)
console.log(data)
```
### 12. List apps
```js
const { activities } = require('koyeb-api-client');
let data = await list_apps(koyeb_api)
console.log(data)
```
### 13. Delete app
```js
const { activities } = require('koyeb-api-client');
let data = await del_app(koyeb_api)
console.log(data)
```

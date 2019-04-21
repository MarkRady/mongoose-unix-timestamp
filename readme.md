# mongoose-unix-timestamp

## Features
  - create created_at column for auto generate time while create this document in unix format
  - create updated_at column for auto generate time while update this document in unix format

### Tech

Mongoose-unix-timestamp uses a number of open source projects to work properly:
* [node.js] - evented I/O for the backend
* [Express] - fast node.js network app framework [@tjholowaychuk]

And of course this is open source and open to contribute on GitHub.

### Installation

```sh
$ cd /path/to/your/app
$ npm install mongoose-unix-timestamp
```
## Usage
```js
const mongoose = require('mongoose');
const Schema = mongoose.Schema;
const unixTimestamp = require('mongoose-unix-timestamp');

const user = new Schema({
	full_name: String,
	email: String,
});

schema.plugin(unixTimestamp);

const model = mongoose.model('User', user);
```

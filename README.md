# REST API Server with Typescript using MongoDB, NodeJS and Express
---

### Screenshot

<img width="317" src="https://user-images.githubusercontent.com/7610219/68885554-ac9e8900-0715-11ea-8b1b-5ca7a5929bc9.png">

### Table of Contents

- [Models](#models)
- [How To Use](#how-to-use)
- [License](#license)
- [Author Info](#author-info)

## Models

##### User schema

```typescript
const UserSchema: Schema = new Schema({
    email: { type: String, required: true, unique: true },
    name: { type: String, required: true },
    pass: { type: String, required: true }
});
```

##### Routes

| Model | Type | Route | Description | Body JSON |
| :---:| :---: | --- | --- | --- |
| USER | GET | /users/all | Get all users | - |
|  | GET | /users/**:id** | Get user by its id | - |
|  | POST | /users/ | Create a new user | User model |
|  | PUT | /users/**:id** | Update an user by its id | User model |
|  | DELETE | /users/**:id** | Delete an user by its id | - |

#### Technologies

- node.js
- express
- mongoose
- angular

## How To Use

#### Installation

Libraries:

```
npm i
```

Run mongo:
```
mongod
```

Run node project:

```
npm start
```
## License

MIT License

Copyright (c) 2019 Izan Pérez Cosano

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

---

## Author Info

Izan Pérez (https://github.com/eperezcosano)
Sheila López (https://github.com/sheilalopez)

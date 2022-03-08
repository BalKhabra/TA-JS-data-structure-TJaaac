```js
let user = {
  name: 'Arya',
  sibling: ['Robb', 'Ryan', 'John'],
};
let allBrothers = ['Robb', 'Ryan', 'John'];
let brothersCopy = user.sibling;
let usename = user.name;
let newUser = user;
```

1. Memory representation

- Create the memory representation of the above snippet on notebook.
- Take a photo/screenshot and add it to the folder `code`

<!-- To add this image here use ![name](./hello.jpg) -->

2. Answer the following with reason:

- `user == newUser;` // true - user value and new user value are equal
- `user === newUser;` // true - copparing doubule equal and triple only if type is different than value is
- `user.name === newUser.name;` // true - address is same
- `user.name == newUser.name;` // true
- `user.sibling == newUser.sibling;` // true
- `user.sibling === newUser.sibling;` // true
- `user.sibling == allBrothers;`// false -points to different address
- `user.sibling === allBrothers;`// false
- `brothersCopy === allBrothers;` // false 
- `brothersCopy == allBrothers;` // false
- `brothersCopy == user.sibling;` // true
- `brothersCopy === user.sibling;` // true
- `brothersCopy[0] === user.sibling[0];` // true it is primitve data type
- `brothersCopy[1] === user.sibling[1];` // true - has the same value of ryan
- `user.sibling[1] === newUser.sibling[1];`// true - points to same primitve data type

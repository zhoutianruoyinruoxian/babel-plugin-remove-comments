

babel-plugin-comments
=========================

Currently it's a babel plugin for remove comments.

## Installation

To install babel-plugin-comments,use npm

```
npm install --save-dev babel-plugin-comments
```

or use yarn

```
yarn add -D babel-plugin-comments
```

## options

-  **remove** (string)  type specifies the type of comments you want to remove.
		
	Possible value：
	```
	- none (default): nothing will be removed;
	
	- all: all comments will be removed;
	
	- line: commentline will be removed(such as: //example);
	
	- CommentLine : same as 'line';
	
	- block: commentblock will be removed(such as: /* example*/);
	
	- CommentBlock: same as 'block';
	
	```
## Example

babel method:

```
  babel.transform(code, { plugins: [[plugin, { remove: 'all' }]] })
```

or babel.config.js:

```
  plugins: [
    [
      'comments',
      {
        remove: 'line',
      }
    ],
  ]
```




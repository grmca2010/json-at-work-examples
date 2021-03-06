Chapter 10 Project Setup
========================
Here's how to create the `myconference` project with Node.


## Contents
- [Create the Project Directory](#create-the-project-directory)
- [Create the Project with `npm init`](#create-the-project-with-npm-init)
- [Install Node Modules](#install-node-modules)
- [Run the ProposalReviewer](#run-the-proposalreviewer)
- [Run the SpeakerNotifier](#run-the-speakernotifier)
- [References](#references)


## Create the Project Directory
First, find a suitable directory for your projects.
`cd ~/projects`

Next, create the `myconference` directory and navigate there:
```
mkdir myconference

cd myconference
```

## Create the Project with `npm init`
Now, use `npm init` to create your Node project.

Your CLI session should look like this:
```
npm init

npm init
This utility will walk you through creating a `package.json` file.
It only covers the most common items, and tries to guess reasonable defaults.

See `npm help json` for definitive documentation on these fields
and exactly what they do.

Use `npm install <pkg> --save` afterwards to install a package and
save it as a dependency in the `package.json` file.

Press ^C at any time to quit.
name: (myconference)
version: (1.0.0)
description: JSON Transform tests.
entry point: (index.js)
test command: mocha test
git repository: ...
keywords: Kafka", Node, JSON
author: Me
license: (ISC) MIT
About to write to .../chapter-10/myconference/package.json:

{
  "name": "myconference",
  "version": "1.0.0",
  "description": "Kafka Producer/Consumer.",
  "main": "index.js",
  "scripts": {
    "test": "mocha test"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/x.git"
  },
  "keywords": [
    "Kafka",
    "Node",
    "JSON"
  ],
  "author": "Me",
  "license": "ISC",
  ...
}


Is this ok? (yes)
```

## Install Node Modules
Next, install the modules we'll need:
```
npm install ajv --save 
npm install handlebars --save 
npm install kafka-node --save 
npm install nodemailer --save 
```

## Run the ProposalReviewer
Run the Proposal Reviewer:
```
node proposalReviewer.js
```

## Run the SpeakerNotifier
Run the Speaker Notifier:
```
node speakerNotifier.js
```


## References
TOC generated by [md-toc](https://www.npmjs.com/package/md-toc).

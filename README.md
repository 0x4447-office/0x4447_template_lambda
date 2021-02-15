# Title me

Describe me

# Consideration for others

- **DO** keep the promises as small as possible. One promise dose only one thing.
- **DO** comment each line to make sure that anyone on the team knows what your code dose.
- **DO** keep your code childish to make it as simple as possible for anyone to understand.

# Environment variables

Copy&Paste the following command to create the `.env` file with all the environment variables needed for the project.

```
printf "%s\n" \
AWS_ACCESS_KEY_ID=DATA \
AWS_SECRET_ACCESS_KEY=DATA \
>> .env
```

# Node

We can control our Node version in NVM (Node Version Manager). To download nvm, run this command
```
$curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```

We use v12.18.4 of Node. Download it and select it.
```
$nvm install 12.18.4
$nvm use 12.18.4
```

# How to run Lambda Locally

```
npm install
```

And once you have all the modules installed you can run:

```
npm run locally
```

# Understanding Our Files

This list explains in details what each file in the project is for, this way you don't have to guess, you can just read the facts.

- `.github`: this folder contains all the files for GitHub to be using to make the page work how we sy it should.
- `.payloads`: this folder contains files that mimic the payloads coming to a Lambda, use it to test your code.
- `.editorconfig`: this file tels your editor how it should work with this repo.
- `.env`: this is where all the environment variables go, and are loaded at startup time.
- `.gitignore`: is a list of files nad folder to ignore by git.
- `.loader`: is the file used by the `npm run build` to execute the code as if it was beeing executed within AWS Lambda. It mimics the environment 1:1.
- `buildspec.yml`: this file contains all the instructions for AWS CodeBuild.
- `index.js`: the initial file that is executed by NodeJS
- `package.json`: this file is used by NPM to know how to behave and what to install.
- `README.md`: you are reding it.

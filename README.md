# README

## Установка npm на Windows Host

Была использована следующая [инструкция](https://phoenixnap.com/kb/install-node-js-npm-on-windows)



## Установка codeceptJS (использована инструкции из вложения к занятию)

[инструкция](https://otus.ru/media-private/73/17/%D0%98%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%86%D0%B8%D1%8F_%D0%BF%D0%BE_%D1%83%D1%81%D1%82%D0%B0%D0%BD%D0%BE%D0%B2%D0%BA%D0%B5_codeceptjs-120120-731744.html)

```javascript
Your environment has been set up for using Node.js 12.18.0 (x64) and npm.

C:\Users\kathe>npm init -y
Wrote to C:\Users\kathe\package.json:

{
  "name": "kathe",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "dependencies": {
    "dotenv": "^8.2.0",
    "minimist": "^1.2.5",
    "mysql": "^2.18.1",
    "mysql2": "^2.1.0",
    "knex": "^0.21.1"
  },
  "devDependencies": {},
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC"
}



C:\Users\kathe>npm install codeceptjs puppeteer --save-dev
npm WARN deprecated request@2.88.2: request has been deprecated, see https://github.com/request/request/issues/3142
npm WARN deprecated har-validator@5.1.5: this library is no longer supported
npm WARN deprecated mkdirp@0.5.4: Legacy versions of mkdirp are no longer supported. Please update to mkdirp 1.x. (Note that the API surface has changed to use Promises in 1.x.)

> puppeteer@5.2.1 install C:\Users\kathe\node_modules\puppeteer
> node install.js

Downloading Chromium r782078 - 149.7 Mb [====================] 100% 0.0s
Chromium (782078) downloaded to C:\Users\kathe\node_modules\puppeteer\.local-chromium\win64-782078
npm WARN kathe@1.0.0 No description
npm WARN kathe@1.0.0 No repository field.

+ puppeteer@5.2.1
+ codeceptjs@2.6.7
added 323 packages from 734 contributors and audited 512 packages in 210.482s

19 packages are looking for funding
  run `npm fund` for details

found 4 low severity vulnerabilities
  run `npm audit fix` to fix them, or `npm audit` for details

C:\Users\kathe>npm audit fix
npm WARN kathe@1.0.0 No description
npm WARN kathe@1.0.0 No repository field.

updated 1 package in 2.751s

19 packages are looking for funding
  run `npm fund` for details

fixed 4 of 4 vulnerabilities in 512 scanned packages

C:\Users\kathe>sudo apt mkdirp update
"sudo" не является внутренней или внешней
командой, исполняемой программой или пакетным файлом.

C:\Users\kathe>mkdirp update
"mkdirp" не является внутренней или внешней
командой, исполняемой программой или пакетным файлом.

C:\Users\kathe>npm mkdirp update

Usage: npm <command>

where <command> is one of:
    access, adduser, audit, bin, bugs, c, cache, ci, cit,
    clean-install, clean-install-test, completion, config,
    create, ddp, dedupe, deprecate, dist-tag, docs, doctor,
    edit, explore, fund, get, help, help-search, hook, i, init,
    install, install-ci-test, install-test, it, link, list, ln,
    login, logout, ls, org, outdated, owner, pack, ping, prefix,
    profile, prune, publish, rb, rebuild, repo, restart, root,
    run, run-script, s, se, search, set, shrinkwrap, star,
    stars, start, stop, t, team, test, token, tst, un,
    uninstall, unpublish, unstar, up, update, v, version, view,
    whoami

npm <command> -h  quick help on <command>
npm -l            display full usage info
npm help <term>   search for help on <term>
npm help npm      involved overview

Specify configs in the ini-formatted file:
    C:\Users\kathe\.npmrc
or on the command line via: npm <command> --key value
Config info can be viewed via: npm help config

npm@6.14.4 C:\Program Files\nodejs\node_modules\npm


C:\Users\kathe>npx codeceptjs init

  Welcome to CodeceptJS initialization tool
  It will prepare and configure a test environment for you

Installing to C:\Users\kathe
? Where are your tests located? ./*_test.js
? What helpers do you want to use? Puppeteer
? Where should logs, screenshots, and reports to be stored? ./output
? Do you want localization for tests? (See https://codecept.io/translation/) English (no localization)
Configure helpers...
? [Puppeteer] Base url of site to be tested http://localhost
? [Puppeteer] Show browser window Yes
? [Puppeteer] Browser viewport size 1200x900

Steps file created at ./steps_file.js
Config created at C:\Users\kathe\codecept.conf.js
Directory for temporary output files created at './output'
Intellisense enabled in C:\Users\kathe\jsconfig.json
TypeScript Definitions provide autocompletion in Visual Studio Code and other IDEs
Definitions were generated in steps.d.ts

 Almost ready... Next step:
Creating a new test...
----------------------
? Feature which is being tested (ex: account, login, etc) demo
? Filename of a test demo_test.js

Test for demo_test.js was created in C:\Users\kathe\demo_test.js

--
CodeceptJS Installed! Enjoy supercharged testing! �
Find more information at https://codecept.io


C:\Users\kathe>npx codeceptjs run --steps
CodeceptJS v2.6.7
Using test root "C:\Users\kathe"

demo --
  test something
  √ OK in 8ms


  OK  | 1 passed   // 2s

C:\Users\kathe>
```
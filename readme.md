# Electron Awesomeness

> Electron Awesomeness is an Electron App to help manage Electron Apps

Run and manage a collection of [awesome electron apps](https://github.com/sindresorhus/awesome-electron) without having to install individual packaged electron binaries. This helps saving disk space and bandwidth not only during installation but during app updates.

## Why this

Personally I prefer to be downloading the source repository for an electron app than downloading the packaged electron app. This is because I already have an electron binary on my computer that I do not like downloading "an embeded electron" for every app that wish to try. So the idea is to run apps like a developer using a global Electron binary. Maybe this has risks and is a bad idea, but I thought I would give this a shot anyways.

Read the reason for this app [here](https://github.com/sindresorhus/awesome-electron/issues/5#issuecomment-155264162).

## How this works

First make sure you have electron installed globally. This app will contain a list of apps that can be checked out or downloaded from github. When it's downloaded, each project would run `npm install --production` to make sure its dependencies are fullfilled. `Electron .` will be ran in each folder to spawn the electron apps.

## Dev

```
$ npm install --production
```

### Run

```
$ npm start
```


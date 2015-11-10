# Electron Awesomeness

> Electron Awesomeness is an Electron App to help manage Electron Apps. Think Steam for Electron Apps.

Run and manage a collection of [awesome electron apps](https://github.com/sindresorhus/awesome-electron) without having to install individual packaged electron binaries. This helps saving disk space and bandwidth not only during installation but during app updates.

## Requirements
- Mac OS X
- git
- npm
- electron

## Why this

Personally I prefer to be downloading the source repository for an electron app than downloading the packaged electron app. This is because I already have an electron binary on my computer, [I do not like downloading](https://github.com/sindresorhus/awesome-electron/issues/5#issuecomment-155264162) "an embeded electron" for every app that I wish to try. Downloading the source could also lower the barrier of entry for developers starting to contribute to open source projects.

So the idea is to run apps like a developer using a global Electron binary. Maybe this has risks and is a bad idea, but I thought I would give this a shot anyways. In contrast to the approach [the discussion on electron/atom runtime seems to be heading](https://github.com/atom/electron/issues/673), this approach is simpler where it lets the developer handle problems, although it would seems more inclined for developers than end-users (like brew perhaps).

## How this works

First make sure you have electron installed globally. This app will contain a list of apps that can be checked out or downloaded from github. When it's downloaded, each project would run `npm install --production` to make sure its dependencies are fullfilled. `Electron .` will be ran in each folder to spawn the electron apps.

### Run

```
$ electron .
```


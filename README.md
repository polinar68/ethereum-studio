# Superblocks Studio

[Superblocks](https://superblocks.com) Studio is an IDE to learn, build and deploy DApps for Ethereum. It's a full browser experience which requires no installs to run.  

Studio has a built in Solidity compiler and Ethereum Virtual Machine, it also works with local and public networks.  

To try it out go to [studio.superblocks.com](https://studio.superblocks.com).

Below is described how to get the Studio PreactJS project setup and running locally.

## License
Superblocks Studio is free software and GPLv3 licensed. See the COPYING file for details.

## Install node modules
Use `yarn` [Yarn](yarnpkg.com/).
```sh
yarn install
```

## Run in dev mode
```sh
make
```

Browse to `http://localhost:8181`. Note that if you use any other hostname/IP than `localhost` run instead `ORIGIN_DEV=http://127.0.0.1 make`.

## Make a production build
```sh
make dist
```

The dist files will be inside `./dist`.

## Bumping version
Set version both in app.js and in manifest.json.
```sh
./bump_version "1.1.0"
```
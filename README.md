# encode-club-weekend-project-4

tokenized ballot full-stack dApp

**note**: this repo has git sub-modules

## cloning this repo

### 3-step method

```bash
git clone <repo-url>

git submodule init

git submodule update
```

### 2-step method

```bash
git clone <repo-url>

git submodule update --init --recursive
```

### 1-step method

```bash
git clone --recurse-submodules <repo-url>
```

## list all submodules attached to this repo

```bash
git submodule
```

### update submodule to latest commits on remote

```bash
git submodule update --remote <sub-module-name>
```

- after running above command, commit this parent repo and push it to remote
- if the above throws an error, run the following

```bash
git pull --recurse-submodules
```

## highlevel overview

We built a full-stack dApp with NestJS server, and Angular client. Several controllers were tested out with OpenAPI based Swagger for the server. Then we used Bootstrap to build out a dApp UI for deploying multiple ballot contracts per poll created by the users. The UI also integrated with Metamask to sign delegations and claim token mints. Overall, we learned quite a bit of TypeScript usage to build client and server apps. We also used ethers library to setup connections with the voting token smart contract and ballot contracts from the client and the server. We used smart contract JSONs and the abi in it to create in-app instances of the contracts deployed on public testnets. 

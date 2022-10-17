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

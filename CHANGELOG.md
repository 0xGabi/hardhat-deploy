# hardhat-deploy

## 0.7.0-beta.28

### Patch Changes

- Breaking change for external field: isolate external deploy script from other artifacts

## 0.7.0-beta.27

### Patch Changes

- fix determinsitic diamond redeployment + verifiability of contracts using libraries

## 0.7.0-beta.25

### Patch Changes

- fix createFixture

## 0.7.0-beta.24

### Patch Changes

- allow multiple tags for --tags + add type param for deployments.createFixture

## 0.7.0-beta.23

### Patch Changes

- fix external deploy exec order + add export-artifacts task to export extended artifacts

## 0.7.0-beta.22

### Patch Changes

- fix types declaration not being published

## 0.7.0-beta.21

### Patch Changes

- remove new types from hardhat/types module
  If you use typescript in your deploy script and import the `DeployFunction` type for example you ll need to update the import

  from

  ```
  import {HardhatRuntimeEnvironment, DeployFunction} from 'hardhat/types';
  ```

  to

  ```
  import {HardhatRuntimeEnvironment} from 'hardhat/types';
  import {DeployFunction} from 'hardhat-deploy/types';
  ```

## 0.7.0-beta.20

### Patch Changes

- fix --reset order to ensure clearing before fetching deployment

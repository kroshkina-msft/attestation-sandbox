## Read Me First

- This sample variant uses libraries installed onto the system using `apt` package tool and cmake. 
- **WARNING**: this variant is NOT complete. It does not employ `vcpkg` as a dependecy manager as it claims.

## Prerequisites
- Dev System with Ubuntu_18.04
- MAA JWT sample token as an input for the verification

## Get Code
```
git clone --recursive git@github.com:kroshkina-ms/attestation-sandbox.git
```

```
cd attestation-sandbox
```

```
git checkout <BRANCH_NAME>
```

```
git submodule update --init
```

## Setup Environemnet and Build Main Branch

```
cd dev-variants/verifier-ubuntu-cmake-vcpkg
```

```
./ubuntu_setup_and_build.sh
```

Check the tool's usage syntax:
```
./out/jwt-verifier
```

Verify quote in JWT:
```
./out/jwt-verifier [options] <jwt-filename>
```

For instance:
```
./out/jwt-verifier -v ~/jwt-samples/jwt.txt
```

![build-status](https://travis-ci.com/theonestack/hl-component-basic-vpc.svg?branch=master)

### Cfhighlander Basic VPC component

```bash

# install highlander gem
$ gem install cfhighlander 

# build and validate standalone component
$ cfhighlander cfcompile --validate custom-vpc

```
### Usage

#### AZ Mappings

AZ region-to-az maps are not needed for this component. 

### Configuration options
Add the below to your app config for private subnets, they are not created by default
  compute:
    allocation: 1
    name: Compute
    type: private
  persistence:
    allocation: 2
    name: Persistence
    type: private
  cache:
    allocation: 3
    name: Cache
    type: private
TBD 

### Parameters
You need to specify AZ's for the max_availabity zones
and also subnet cidr's for each subnet public or private
e.g.
PublicSubnet0cidr:  10.0.0.0/27

TBD

### Configuration options

TBD

### Outputs

TBD

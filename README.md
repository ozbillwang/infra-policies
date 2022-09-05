# infra-policies
policies from cloud custodian

ref: [AWS + AZURE using AzureDevOps & Cloud Custodian | Open Source DevOps, DevSecOps, Azure Pipelines](https://www.youtube.com/watch?v=ElvHiZU8hRc)

### Commands for reference

Install custodian

```
pip install c7n-azure
```

common commands

```
# validate the policy
$ custodian validate policies/az-nic-not-attached.yml

# dry rn
$ custodian run --dry-run -s out policies/az-nic-not-attached.yml

# see reprot
$ custodian report s out policies/az-nic-not-attached.yml --format grid
```

# GitHub Action - AMI Builder

## Example:

```yml
- name: Build AMI
  uses: acerorg/gha-ami-builder@v1
  with:
    AWS_ACCOUNT: 111111111111
    AWS_REGION: ap-southeast-2
    AWS_ACCESS_KEY_ID: XXXXXXXXXXXXXXXXXXXX
    AWS_SECRET_ACCESS_KEY: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
    BILLING_ID: MY_BILLING_ID
    EC2_NAME: PROJECT_NAME/REPO_NAME/AMI-Builder
    VPC_ID: vpc-00000000
    SUBNET_ID: subnet-00000000000000000 # Atmosphere-UAT2 app Private (ZoneA)
    SECURITY_GROUP_ID: sg-xxxxxxxxxxxxxxxxx # Atmosphere-UAT2-App-Networksappsg4D02FC6B-P5PBSXZ7FYDQ
    KEY_PAIR: MY_KEY_PAIR
    EC2_INSTANCE_PROFILE: Atmosphere-UAT2-App-BuildAmiLaunchTemplateProfileDE4DF5E1-2Y0LEDVtyhEh
    INSTANCE_TYPE: t3.medium
    INSTANCE_DISK_SIZE: 30
```

# Exploring Packer

### Purpose
- Project explores creation of amazon machine images using packer tool.

### Requirements
- [ ] Packer Executable (path established)
- [ ] AWS account with permission to build ami and launch with EC2
- [ ] AWS Cli deploying image from cmdln/terminal

### Implementation (Create AMI)
+ Example 1
    - `cd ami`
    - `packer validate ami/ubuntu_basic.json` then `packer build ami/ubuntu_basic.json`
+ Example 2
    - Export private AWS credentials in terminal
    - - `cd ami`
    - `packer validate ubuntu_script.json` then `packer build ubuntu_script.json`
+ NOTE
    - Record the ami-id once the build has successfully completed or check AWS console for newly created amis

### Documentation
- [Packer Tutorial](https://learn.hashicorp.com/tutorials/packer/getting-started-build-image)

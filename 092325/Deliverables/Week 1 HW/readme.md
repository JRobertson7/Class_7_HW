Class 7:EC2

Objective- building an EC2 with script

template- https://github.com/MookieWAF/bmc4/blob/main/ec2scrpit

steps
1. create NEW security group, DO NOT USE DEFAULT
2. create EC2 
3. copy public DNS, make it into link via http://

Teardown
1. go to instances, select made instances, instance state & terminate instances
2. go to security groups, select made security group, select actions & delete security group
3. go to key pairs, select made key pair, select actions & delete key pairs
4. deleting security groups & key pairs are optional




notes
- make key pair can keep same name as instance
- both security groups and key pairs are under same tab (Network & Security)
- make sure to make usable link type http:// before proceeding
- make tags, its easier for team to keep track of them
- place screenshots in class 7 folder labeled HW (make new folder)
# ProxyCannon-2025
This repo is a fork of a revival script by yg-ht which is a fork of a single script by Shellntel in their repo "scripts". 

### Why bother

AWS has updated its terms to state that outbound use of API Gateway is prohibited and I want to rotate my source IP.

## Command-line syntax

````
-id, default='ami-d05e75b8', Amazon AMI image ID
-t, default='t2.nano', Amazon AMI image type
--region, default='us-east-1', Select the region
-r, Enable Rotating AMI hosts
-b, Enable multi-path cache busting
-m, Disable link state monitor
-v, Enable verbose logging
--name, Set the name of the instance in the cluster
-i, default='detect', Interface to use, default will result in detecting the default gateway and using that
-l, Enable logging of WAN IP's traffic is routed through

num_of_instances, The number of instances you'd like to launch.
````

python proxycannon.py 4 -r

## Install

```pip3 install -r requirements.txt```

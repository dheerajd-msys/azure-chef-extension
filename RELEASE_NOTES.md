<!---
This file is reset every time a new release is done. The contents of this file are for the currently unreleased version.

Example Note:

## Example Heading
Details about the thing that changed that needs to get included in the Release Notes in markdown.
-->

# azure-chef-extension 1210.12.102.1000 release notes:
In this release we have added extension support for RHEL platform. We have also added an option `validation_key_format` which can be provided in either ARM template or `publicconfig.config` file as explained [here](https://github.com/chef-partners/azure-chef-extension#azure-chef-extension-usage).
Value of `validation_key` should be provided accordingly.

See the [CHANGELOG](https://github.com/chef-partners/azure-chef-extension/blob/master/CHANGELOG.md) for a list of all changes in this release, and review.

More information on the contribution process for Chef projects can be found in the [Chef Contributions document](https://docs.chef.io/community_contributions.html).

## azure-chef-extension on Github
https://github.com/chef-partners/azure-chef-extension

##Features added in azure-chef-extension 1210.12.102.1000
* [azure-chef-extension #115](https://github.com/chef-partners/azure-chef-extension/pull/115) Decrypting validation key if it's provided in Base64encoded format
* [azure-chef-extension #116](https://github.com/chef-partners/azure-chef-extension/pull/116) Added AzureChefExtension support for RHEL platform

## Known Issues
* When update is done for extension on windows and linux with autoUpdateClient=false, update doesn't happen(which is correct) but user doesn't get the actual error message. WAagent starts enable command and error logs show that enable command has failed.

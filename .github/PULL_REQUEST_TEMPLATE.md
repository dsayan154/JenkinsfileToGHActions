# Deployment note

Please be aware that all changes in a Pull Request will be deployed at the same time, and there is no gating.  This means that if you need to make a change to both a UAT and a Production environment, and the production should not be immediately deployed, you must create two seperate Pull Requests.

# Gentle Reminder
Before you create your PR take a look at our checklist:
- [ ] If you added a new configuration parameter, did you update the config template?
    * [Ex. Config Template](https://github.com/providenceinnovation/ecp-customer-config/blob/master/config/forq-account/v1/config.json.tmpl)
  [ ] If you added a new configuration parameter, did you add that to the common `customValues.yaml.topopulate` file?
    * [customValues.yaml.tmpl](https://github.com/providenceinnovation/ecp-customer-config/blob/master/config/common/customValues.yaml.topopulate)
- [ ] If you added an external / 3rd party service dependency, did you update the dependency template?
    * [Ex. Dependencies Template](https://github.com/providenceinnovation/ecp-customer-config/blob/master/config/forq-account/v1/dependencies.yaml.tmpl)
- [ ] Did you update the config version for your service [here](https://github.com/providenceinnovation/ecp-customer-config/blob/master/requirements-assets.yaml)?
- [ ] Should the new configuration or asset be replicated in each cluster? Is it done?

> Devex team.

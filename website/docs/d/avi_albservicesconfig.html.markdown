############################################################################
# ------------------------------------------------------------------------
# Copyright 2020 VMware, Inc.  All rights reserved. VMware Confidential
# ------------------------------------------------------------------------
###

---
layout: "avi"
page_title: "AVI: avi_albservicesconfig"
sidebar_current: "docs-avi-datasource-albservicesconfig"
description: |-
  Get information of Avi ALBServicesConfig.
---

# avi_albservicesconfig

This data source is used to to get avi_albservicesconfig objects.

## Example Usage

```hcl
data "avi_albservicesconfig" "foo_albservicesconfig" {
    uuid = "albservicesconfig-f9cf6b3e-a411-436f-95e2-2982ba2b217b"
    name = "foo"
}
```

## Argument Reference

* `name` - (Optional) Search ALBServicesConfig by name.
* `uuid` - (Optional) Search ALBServicesConfig by uuid.

## Attributes Reference

In addition to all arguments above, the following attributes are exported:

* `asset_contact` - Information about the default contact for this controller cluster.
* `feature_opt_in_status` - Information about the portal features opted in for controller.
* `ip_reputation_config` - Default values to be used for ip reputation sync.
* `polling_interval` - Time interval in minutes.
* `portal_url` - The fqdn or ip address of the customer portal.
* `proactive_support_defaults` - Default values to be used during proactive case creation and techsupport attachment.
* `split_proxy_configuration` - Split proxy configuration to connect external pulse services.
* `use_split_proxy` - By default, use system proxy configuration.if true, use split proxy configuration.
* `uuid` - Field introduced in 18.2.6.


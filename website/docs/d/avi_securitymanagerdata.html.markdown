############################################################################
# ------------------------------------------------------------------------
# Copyright 2020 VMware, Inc.  All rights reserved. VMware Confidential
# ------------------------------------------------------------------------
###

---
layout: "avi"
page_title: "AVI: avi_securitymanagerdata"
sidebar_current: "docs-avi-datasource-securitymanagerdata"
description: |-
  Get information of Avi SecurityManagerData.
---

# avi_securitymanagerdata

This data source is used to to get avi_securitymanagerdata objects.

## Example Usage

```hcl
data "avi_securitymanagerdata" "foo_securitymanagerdata" {
    uuid = "securitymanagerdata-f9cf6b3e-a411-436f-95e2-2982ba2b217b"
    name = "foo"
}
```

## Argument Reference

* `name` - (Optional) Search SecurityManagerData by name.
* `uuid` - (Optional) Search SecurityManagerData by uuid.

## Attributes Reference

In addition to all arguments above, the following attributes are exported:

* `app_learning_info` - Information about various applications.
* `name` - Virtualservice name.
* `tenant_ref` - It is a reference to an object of type tenant.
* `uuid` - Virtualservice uuid.


---
title: Ghostfolio
description: Ghostfolio Widget Configuration
layout: ../../../layouts/MainLayout.astro
---

Authentication requires manually obtaining a Bearer token which can be obtained by visiting `http://<ghostfolio_host>:<ghostfolio_port>/api/v1/auth/anonymous/<SECURITY_TOKEN_OF_ACCOUNT>`.

*Note that the Bearer token is valid for 6 months, after which a new one must be generated.*

Allowed fields: `["gross_percent_today", "gross_percent_1y", "gross_percent_max"]`

```yaml
widget:
    type: ghostfolio
    url: http://ghostfoliohost:port
    key: ghostfoliobearertoken
```
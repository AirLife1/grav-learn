---
title: Invalid Security Token
taxonomy:
    category: docs
---


**Problem:** You get this error in the Admin panel when logging in on performing opertions

There are a few possible causes of the problem, all linked to the Session:

- Try **reloading** your browser to get a fresh token

- Try clearing your browser session cookies, Try logging out and back in.`session.secure: true` set in Grav's `system.yaml`

- Ensure you running under SSL using and HTTPS URL if you have

- Check that PHP has the correct tmp path set up. This can be set in PHP directly, or by setting Grav's `system.yaml` `session.path` setting (it can be also set via Admin, in the System Configuration) [Reported issue](https://github.com/getgrav/grav-plugin-admin/issues/958)

- Make sure your web server config is right and includes the query string [Reported issue](https://github.com/getgrav/grav-plugin-admin/issues/893)

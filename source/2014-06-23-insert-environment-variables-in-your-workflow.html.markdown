---
title: Insert Environment Variables in your Workflow
date: 2014-06-23 14:43 UTC
tags: concrete-update, site-update
authors: Viktor Benei|viktor.benei@gmail.com
---

You could always insert Environment Variables into your Workflow's step inputs but from now on you can use our quick inserter popup.

All you have to do is:

1. Go to your App's **Workflow tab**
2. Click on a Step to expand it
3. Click on **Insert Variable** under the input field you want to insert an Environment Variable into
4. In the presented popup click on a variable

![Example Insert Variable popup](insert-variable-into-step-input-1.png)

This will insert the selected Environment Variable key into the input field. During an actual Build the Environment Variable's value will replace the key.

For example the *$CONCRETE_STEP_DIR* key will be replaced with the actual path of the Step directory.

> Note: the Insert Variable Popup lists the Environment Variables which are set by the Concrete Build (for example the build's and the app's URL) automatically **and** the Environment Variables which are exported from previous Steps.

> For example the *Xcode Build* Step exports a *$CONCRETE_BUILD_STATUS* variable, which will store whether the Build was successful or not.
> For more details on Step exported Environment Variables check out the Concrete DevCenter's [Step Development](http://devcenter.concretebuilder.io/step-dev.html) page.
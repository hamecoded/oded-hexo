---
title: Test your puppet
date: 2016-08-03 17:00:24
tags: 
 - puppet
 - devops
---


## How to test your puppet script
When working with a deployment environment that does many things beside of running your puppet file, you sometimes want to debug and test you puppet manifest or module in as little as time possible. The following is a quick steps to have that achieved using the command ``puppet apply``.
1. Go to the machine inwhich you'd like the puppet to be ran.
2. Create a ``modules`` directory and copy you puppet modules into that directory.
3. Create a ``manifest.pp`` in the same directory which contains the ``module`` directory.
4. Execute 
```bash
	puppet apply manifest.pp --modulepath=modules/
```
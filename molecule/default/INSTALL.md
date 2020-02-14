---
title: 'Test environment setup'
show_comments: true
show_feedback: true
---

# Docker driver installation guide

## Requirements

* Docker Engine

## Install

Please refer to the [Virtual environment](https://virtualenv.pypa.io/en/latest/) documentation for installation best
practices. If not using a virtual environment, please consider passing the widely recommended `--user` flag when 
invoking `pip`. More information 
[here](https://packaging.python.org/tutorials/installing-packages/#installing-to-the-user-site).

```shell script
pip install molecule[docker]
```

---
layout: post
title: Opencv-Python bug
---

## Environment

* Mac OS
* Python 3.6.1
* Opencv 3.2.0

## Bug Description

> BUG: The current event queue and the main event queue are not the same. Events will not be handled correctly. This is probably because _TSGetMainThread was called for the first time off the main thread.

## Solution

> Reinstall Opencv with [--with-ffmpeg flag]

### Contact me

[foleevora@gmail.com](mailto:foleevora@gmail.com)

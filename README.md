# Drive

**Primary Maintainer:** Brian Smith (brian.smith@maidsafe.net)

|Crate|Linux/OS X|Windows|Coverage|Issues|
|:---:|:--------:|:-----:|:------:|:----:|
|[![](http://meritbadge.herokuapp.com/drive)](https://crates.io/crates/drive)|[![Build Status](https://travis-ci.org/maidsafe/drive.svg?branch=master)](https://travis-ci.org/maidsafe/drive)|[![Build status](https://ci.appveyor.com/api/projects/status/so3q2w6g8vey2avl/branch/master?svg=true)](https://ci.appveyor.com/project/MaidSafe-QA/drive/branch/master)|[![Coverage Status](https://coveralls.io/repos/maidsafe/drive/badge.svg)](https://coveralls.io/r/maidsafe/drive)|[![Stories in Ready](https://badge.waffle.io/maidsafe/drive.png?label=ready&title=Ready)](https://waffle.io/maidsafe/drive)|

| [API Documentation - master branch](http://maidsafe.net/drive/master) | [SAFE Network System Documentation](http://systemdocs.maidsafe.net) | [MaidSafe website](http://maidsafe.net) | [SAFE Network Forum](https://forum.safenetwork.io) |
|:------:|:-------:|:-------:|:-------:|

## Overview

A cross platform [virtual file-system in userspace](http://en.wikipedia.org/wiki/Filesystem_in_Userspace) (drive) that will appear as a regular drive on the operating system. The interface is a POSIX-like API and this is exposed in every OS. May include a webdav interface where possible.

IOS and Android…etc… may require a driverless option, further consideration will also be required (webdav ?) to provide the same cross platform/OS compatibility.

This drive can provide a blocking call to be used as a stand alone application, or a threaded call to enable a drive to be mounted from any application.

## Prerequisites

### Linux

Requires fuse dev files in ubuntu `sudo apt-get install libfuse-dev`

### OS X

Requires osxfuse (easiest method is to use Homebrew and `brew install osxfuse`

### BSD

Likely working [Puffs](http://www.netbsd.org/docs/puffs/) and will require fuse-development library installed, but requires tests and CI integration.

### Windows

Currently unimplemented and will require the [windows driver frameworks](https://github.com/Microsoft/Windows-Driver-Frameworks) as per these [examples](https://github.com/Microsoft/windows-driver-samples)

## Todo Items
- [ ] Finalise API
- [ ] Confirm Bsd
- [ ] Provide simple example (mirror)
- [ ] API version 0.0.8
- [ ] Add windows driver version
- [ ] API version 0.0.9
- [ ] Webdav integration
- [ ] API version 0.1.0
- [ ] Investigate midipix and DokanY.

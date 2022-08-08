---
layout: post
title: "Installation and Tutorial"
author: "Tim Davis"
categories: documentation
tags: [documentation,sample]
image: KinMS_in_action.png
---

KinMSpy is designed with Python users in mind, and is hopefully easy to install and use. For most use cases you will want to follow the directions under "Normal User". If you are a power-user who wants to do something out of the ordinary then follow the "Power User" instructions. Both user types have tutorials avalible (see below).


<font size=5><u>Normal User</u></font>
If you are a new user, and/or you don't expect to need any advanced features then you will want the KinMS_fitter package. This installs the base KinMS routines, and wraps them in a user-friendly way to get you fitting datacubes in the minimum possible time.

<font size=4><u>Install</u></font>

KinMS_fitter can be installed with `pip install kinms-fitter`. Alternatively you can download the code from [GitHub](https://github.com/TimothyADavis/KinMS_fitter), navigate to the directory you unpack it too, and run `python setup.py install`.

<font size=4><u>Tutorial</u></font>

An iPython notebook tutorial on KinMS_fitter can be found here: [KinMS_fitter tutorial](https://github.com/TimothyADavis/KinMS_fitter/blob/main/kinms_fitter/docs/KinMS_fitter_tutorial.ipynb)


<font size=5><u>Power User</u></font>

If you are a power user then you may just want the base KinMS routines without the fitter, in order to roll your own analysis code. Note- if you already installed the fitter then there is no need to install KinMS seperately- you already have everything you need to follow the tutorials below.

<font size=4><u>Install</u></font>
KinMS can be installed with `pip install kinms`. Alternatively you can download the code from [GitHub](https://github.com/TimothyADavis/KinMSpy), navigate to the directory you unpack it too, and run `python setup.py install`.
    
<font size=4><u>Tutorials</u></font>

To understand the basics of the base KinMS rotuines a tutorial can be found here: [KinMS simple tutorial](https://github.com/TimothyADavis/KinMSpy/blob/master/kinms/docs/KinMS_example_notebook.ipynb)

A further suite of examples can be found in examples/KinMS_testsuite.py, which can be modified and updated for most use cases. To run these tests you can run the following commands from within python on KinMS is installed:

```
from kinms.examples.KinMS_testsuite import *
run_tests()
```

If you need go through the nuts and bolts of fitting, see the walk through here: [Example fitting tutorial](https://github.com/TimothyADavis/KinMSpy/blob/master/kinms/docs/KinMSpy_tutorial.ipynb)



### Bugs and further assistance
If you find any bugs while using KinMS, or have feature requests, please either raise an issue on the respective [github]({{ site.github.url }}/about), or [contact me directly]({{ site.github.url }}/contact). Similarly, I am very happy to assist with all aspects of using KinMS- feel free to [get in touch]({{ site.github.url }}/contact)!

### Mailing List

Once you have KinMS installed and working you may wish to join the mailing list, so you can be kept up to date with major releases and bugs. [Simply contact me]({{ site.github.url }}/contact) - you will never be spammed, or your details sold!
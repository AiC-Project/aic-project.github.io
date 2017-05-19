---
layout: default
title: {{ site.name }}
lang: en
langTitle: English
ref: home
---

## Improve Android development quality and costs 

AiC 2.0 goal is to ease large scale review for Android applications. 

Technically it means to offer an answer to physical devices (smartphones, tablets, Connected TVs) and Android versions multiplication, thanks to an easy to use, fully featured, Cloud-oriented solution. 

This solution relies heavily on the provision of Android virtual machines.

One of the advantage for this approach is to accelerate Android test environments deployment and configuration time while dramatically reducing the investment and maintenance of a physical devices fleet.

## Run manual or automated Android tests

The Saas AiC 2.0 solution introduces two main features to its user: the live campaign and the asynchronous campaign.

### Live campaign

Thanks to the live campaign, you can interact with an Android virtual machine from the AiC 2.0 web interface directly in your browser without any additional plugins.

![AiC Live Campaign](/img/AiC_live_campaign_640.gif){:class="img-responsive"}

__In a few words, _it is Android in the browser.___


Among the features of the live campaign :

- choice of Android version (phone or tablet, KitKat or Lollipop)
- configuration of screen resolution and pixel density
- real time apks installation
- Android sensors stimulation from the web interface (including GSM and Wifi)
- possibility to switch to full screen or to adapt the view to the size of your screen

### Asynchronous Campaign

Using the asynchronous campaign, you can schedule a campaign that will run your UiAutomator or AiC 2.0 tests on a large scale of configurable Android virtual instances. The virtual instances are visually accessible during the execution of the test set, and the results are then presented in the Junit format.

![AiC Async Campaign](/img/AiC_async_campaign_640.gif){:class="img-responsive"}

__In a few words, _it is Android in the Cloud.___


Among the features of the asynchronous campaign :

- possibility of using the native tests UiAutomator or the dedicated DSL AiC 2.0
- choice of Android versions on which to run the tests
- real-time notifications of the campaign's progress
- virtual instances accessible during test execution
- campaign results saved and presented in Junit format


### The AiC 2.0 DSL
The AiC 2.0 DSL is a project-specific innovation allowing an user to express a functional test in natural language close to Gherkin. Compared to the traditional Android test solutions (UiAutomator, Espresso, Junit), the AiC 2.0 DSL allows to express functional tests while specifying the state of the system sensors (including Bluetooth, NFC).

{% highlight gherkin%}
Feature: "Example feature"

    Scenario: "Minimal example scenario"
        Set battery level at 5
        Check if "Low battery" exists
    End

    Scenario: "More complex example scenario"
        Click on “Sensor”
        Scroll from "Picture" to "Photometer"
        Scroll from "Photometer" to "Gyroscope
        Click on "Proximity Sensor"
        Type "Value is going to change..." into "R.id.input_exemple"
        Set sensor "TYPE_PROXIMITY" at 18
        Replace "It's working !" into "R.id.input_exemple"
        Click on "Proximity Sensor"
        Scroll from "Proximity Sensor" to "Bluetooth"
        Click on "Ambient Thermometer"
    End

End
{% endhighlight %}


In summary, the AiC 2.0 DSL allows to :

- express Android functional tests in  Gherkin-like natural language
- describe the state of the Android system dynamically within the test sequence
- compile a test apk that can then be used in an asynchronous campaign


## Using the AiC 2.0 solution

There are two ways to use AiC 2.0 :
- You can use beta version hosted on FIT UPMC Cloud Openstack testbed. You can access it here:  [AiC 2.0](https://aic.onelab.eu:8443/), it is free of charge, but you will need [to create OneLab account](https://portal.onelab.eu/register)
- Install the solution from [the Github sources](https://github.com/AiC-Project)


## Consortium and Funding

### The partners behind the project
The AiC 2.0 project consortium brings together the following industrial and academic partners :

- Alter Way, industrial partner and project pilot
- Zenika, industrial partner
- Liafa, academic partner
- Lip6, academic partner
- Thales, large user

![AiC Partners Logo](/img/AiC_partners_logo.png){:class="img-responsive"}


### Funding actors
The AiC 2.0 project is a collaborative R&D project resulting from the call for projects [FUI #16](http://www.systematic-paris-region.org/fr/actualites/le-16e-appel-a-projets-fui-retient-12-projets-labellises-par-systematic-paris-region).

The FUI (Unified Interministerial Funds) is a program aiming to support applied research to help develop new products and services that can be put on the market in the short or medium term.


It allows to finance "collaborative" R&D projects (involving, for example, large companies, SMEs and laboratories), following their labeling by the competitiveness clusters.

The financing is then managed by the BPI in association with the communities, for the project AiC 2.0, the Ile de France region.

![AiC Financial Logo](/img/AiC_financial_logo.png){:class="img-responsive"}


### Open Source Effort
The code produced in the project will be released under open source license, in accordance with [the GTLL agreement](http://www.systematic-paris-region.org/fr/logiciel-libre/propos/charte).

### FUI Program Calendar
Started in December 2013, the project program is underway and will stop in October 2017.

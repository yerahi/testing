# Open Web Launch

## Introduction

For years, Java Web Start has been used as deployment vehicle for Java Desktop applications. As of Java 9, however, the feature has been deprecated – and in Java 11, Java Web Start has been removed completely.

Oracle has pitched several other deployment scenarios, but many existing projects, products and components have trouble to make that change in time, or at all for that matter. Open Web Launch has been created to fill the gap this change of functionality leaves behind.

**Note:** 

Open Web Launch can work with any Java version of any provider \(Oracle, OpenJDK or IBM\), with JREs and JDKs. Please note that Open Web Launch will not address any Java-compatibility issues for the Java applications it serves – this is the responsibility of their manufacturer. The prime goal for Open Web Launch is to run any application as configured in its JNLP file against a Java version which may officially no longer support Java Web Start.)

## Usage Scenarios

### JNLP files

This scenario makes sure double clicking a JNLP file in the explorer opens it, downloading required resources, and starting the application as instructed.

**Note:** 

This scenario needs the Open Web Launch \(OWL\) application to be installed.

### JNLP URLs

This scenario takes care of intercepting JNLP file URLs that are clicked on in a browser and redirects their handling to the Open Web Launch application, downloading required resources, and starting the application as instructed.

**Note:** 

This scenario needs the OWL browser extension and application to be installed.

### JNLP protocol

This scenario redirects every URI starting with `jnlp:` or `jnlps:` and redirects their handling to the Open Web Launch application, downloading required resources, and starting the application as instructed.

**Note:** 

This scenario needs the OWL application to be installed.

## Installation

An appropriate Java version needs to be installed on the system for OWL to work. Certificates required by a Java application need to be imported.

There are two ways to install OWL on your system – either through a setup \(executable\) or through a browser extension.

### Setup

#### User install

Run the setup for the current user only.

-   Point at the Java you want to use for all Web Start applications.

-   Select whether you want to make OWL the default for opening JNLP files.

-   Select whether you want to register the JNLP and JNLPS protocol for Open Web Start.

-   Select whether you want to show the Java console when opening JNLP files.

#### Admin install

Administrative privileges are required.

Run the setup so that all users on the system have access to it.

-   Point at the Java you want to use for all Web Start applications.

-   Select whether you want to make OWL the default for opening JNLP files.

-   Select whether you want to register the JNLP and JNLPS protocol for Open Web Start.

-   Select whether you want to show the Java console when opening JNLP files.  

#### Silent install

There is an option to run the setup silently, which uses the defaults:

`setup /s`

#### Uninstall

OWL can be uninstalled from the Control Panel or from a shortcut in the Start Menu. 

### Browser extension

#### Chrome

The extension for Chrome is available in the Chrome Web Store from [https://chrome.google.com/webstore/detail/open-web-launch/pmmlhpkdpbddohdbnjinopbkmlcnjnhc](https://chrome.google.com/webstore/detail/open-web-launch/pmmlhpkdpbddohdbnjinopbkmlcnjnhc).

#### **Firefox**

The add-on for Firefox is available on the Mozilla site from [https://addons.mozilla.org/en-US/firefox/addon/open-web-launch/](https://addons.mozilla.org/en-US/firefox/addon/open-web-launch/).

## Appendix

### Frequently Asked Questions

#### What operating systems does Open Web Launch support?

Open Web Launch is available for Windows, macOS and Linux.

#### Are there 32 and 64-bit versions available?

The default download is 64-bit. 32-bit can be created on request.

### Supported keywords

|Element|   |Attribute|Values / Description|
|-------|---|---------|--------------------|
|**information**| | | |
| |icon| | |
| |shortcut| | |
|**title**| | | |
| |vendor| | |
| |homepage| | |
| |description| | |
|**application-desc**| | | |
|**resources**| | | |
| | |os|windows, darwin, linux|
| | |arch|amd64, x86|
| |jar| | |
| | |href| |

### Links

#### JNLP definition

[https://docs.oracle.com/javase/tutorial/deployment/deploymentInDepth/jnlp.html](https://docs.oracle.com/javase/tutorial/deployment/deploymentInDepth/jnlp.html)

#### JNLP examples

[https://docs.oracle.com/javase/tutorial/uiswing/examples/misc/index.html](https://docs.oracle.com/javase/tutorial/uiswing/examples/misc/index.html)

#### Chrome Extension

[https://chrome.google.com/webstore/detail/open-web-launch/pmmlhpkdpbddohdbnjinopbkmlcnjnhc](https://chrome.google.com/webstore/detail/open-web-launch/pmmlhpkdpbddohdbnjinopbkmlcnjnhc)

#### Firefox Add-on

[https://addons.mozilla.org/en-US/firefox/addon/open-web-launch/](https://addons.mozilla.org/en-US/firefox/addon/open-web-launch/)

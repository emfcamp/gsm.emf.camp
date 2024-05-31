---
title: GRPS
description: >
  Connecting to the Internet over the EMF GSM network
---

GPRS is experimentally available on the EMF GSM network, and any APN should work (`internet` is fine).

# WAP Gateway

**The WAP gateway is not hosted by the EMF GSM team, and is hosted by [Billy](https://billy.wales).**

For devices that need a WAP Gateway (such as the Nokia 6310i and Nokia 6100), a third party of Kannel is available at `129.151.64.135`.
The following steps are written with a Nokia device in mind, but should be useful for anyone trying to connect with the WAP gateway.

1. Press Menu, select Services, and Settings.
2. Select Active service settings.
3. Scroll to the set you would like to edit and activate, and press *Activate*.
4. Select *Edit active service settings*, and enter the following information:
    - Settings' name: "EMF" or similar name.
    - Homepage: `http://wap.billy.wales` (or similar WML homepage)
    - Session Mode: Permanent
    - Connection Security: Off
    - Data Bearer: GPRS
    - GPRS Connection: When needed (or Always, but this may drain battery!)
    - GPRS access point: internet
    - IP address: `129.151.64.135`
    - Authentication Type: Normal
    - Login Type: Automatic
    - User name / password: (leave blank)
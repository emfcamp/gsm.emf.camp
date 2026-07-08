---
title: GPRS
description: Connecting to the Internet over the EMF GSM network
---

{{% alert title="Important" color="warning" %}}
GPRS data bandwidth is very limited - please do not enable this if you are using this SIM in a modern smartphone as the background services will use up a lot of network capacity.
Instead use our LTE network for mobile data on modern smartphones, you will still fall back to GSM for phone calls.
{{% /alert %}}

You will need to enable GPRS for your SIM in order to be able to use data on 2G.

[GPRS](https://en.wikipedia.org/wiki/GPRS) is experimentally available on the EMF GSM network, and any APN should work (`internet` is fine).

{{< figure src="/images/gprs-speed.jpg" caption="Screenshot of speedtest on EDGE" alt="17.9kB/s download, 7.62kB/s upload, 595ms ping, 344ms jitter." width="300px" >}}

## WAP Gateway

For devices that need a WAP Gateway (such as the Nokia 6310i and Nokia 6100), a third party installation of Kannel is available to use.

The following steps are written with a Nokia device in mind, but should be useful for anyone trying to connect with the WAP gateway.

1. Press Menu, select Services, and Settings.
2. Select Active service settings.
3. Scroll to the set you would like to edit and activate, and press *Activate*.
4. Select *Edit active service settings*, and enter the following information:
    - Settings' name: "EMF" or similar name.
    - Homepage: `http://m.phones.emf.camp`
    - Session Mode: Permanent
    - Connection Security: Off
    - Data Bearer: GPRS
    - GPRS Connection: When needed (or Always, but this may drain battery!)
    - GPRS access point: internet
    - IP address: `92.118.29.108`
    - Authentication Type: Normal
    - Login Type: Automatic
    - User name / password: (leave blank)

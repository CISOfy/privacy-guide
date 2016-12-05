# Browser Security

With many applications being available via the browser, the security and privacy settings of the browser come into play.

Before knowing how to properly configure the browser, it is valuable to understand the risks of using a browser. In particular interesting is what happens without precautions.

## Fingerprints

* [Click](https://clickclickclick.click/)
* [Webkay](http://webkay.robinlinus.com/)

## IP Addresses

When browsing the web, usually two or more IP addresses are involved. Each of these addresses can be statically or dynamically assigned. Common examples include the private address on your internal network. Then there are public addresses that are routable on the internet, like the IP address of the router, a VPN server, or tor exitnode.

One of the risks with IP addresses is that they might become known to the parties that exchange data and those who forward any data packets. 

Public addresses are hard to hide, as in the end some system needs to request the web page. By using a VPN service, the (shared) IP address of the network can be hidden. That is, if the right measures are implemented. See the section about WebRTC for more information.

Private addresses (10.x.x.x, 172.16.x.x, 192.168.x.x) are possibly the most sensitive, as they may point to the specific system within a company or personal network.

### Testing IP leaking

* [ipleak.net](https://ipleak.net/)

### WebRTC

Let's start with a quote of what WebRTC is: "WebRTC is a free, open project that provides browsers and mobile applications with Real-Time Communications (RTC) capabilities via simple APIs. The WebRTC components have been optimized to best serve this purpose."

This set of capabilities are programmed to make it as easy as possible to communicate. Unfortunately this may result in leaking too much information. Unfortunately many users who are behind a VPN, are still leaking their own end-point, including up to the private IP address on the network.

#### What You Can Do

Disable some parts of WebRTC with a browser plugin
* [Chrome] WebRTC Leak Prevention addon


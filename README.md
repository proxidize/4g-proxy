# Create or build your own 4g mobile proxy

How to create a 4G/LTE mobile proxy from a USB modem/dongle and a Raspberry Pi using Proxidize free script. With this script, making your own 4G mobile proxies is easier than ever.

This the Proxidize free script, created to show users that making your own 4G proxies can be very simple.

This script has minimal features and is only intended to be a demo explanation to show how simple the process of creating 4G proxies is.

To install the script, get the hardware ready, and run it.

You find our full guide here: https://proxidize.com/how-to-make-a-4g-mobile-proxy/

Learn more about Proxidize: https://proxidize.com

The script works by routing the connection from the default router connection to the mobile network connected by the 4G dongle. This is done through a mixture of ip and iptables rules that ensure the routing is done correctly.

4G mobile proxies are proxies created from the connection to a mobile, most often by 4G modems but this can also be done via regular phones. You can use our app to achieve this called Proxidize Android: https://play.google.com/store/apps/details?id=com.proxidize


Thank to CGNAT, 4G mobile proxies are superior to every other type of proxy as it camouflages the bots and/or automation software. This happens because the public IPV4 address used by the 4G mobile proxy is simultaneously used by hundreds or real users which makes IP bans a lot more difficult since 99% of the time the traffic fingerprint coming from the IP address will look 100% normal no matter how aggressive your automation settings are.

Please note, not all mobile carriers do use CGNAT, but the vast majority of them do. You can check this by going into your phone setting and if your IP starts with 10.xx.xx.xx then you are most likely connected to a CGNAT network.

This script requires both a 4G mobile connection and a regular router connection. This is one of the downsides of CGNAT technology as it makes it impossible for a single device to control any particular port.

This is not something you need to worry about with this script, since it's designed to be used internally only.


The way the Android phones bypasses this issue is by initiating a connection to an external server which then makes a port available for this particular device to use. This is done through reverse SSH tunnels.

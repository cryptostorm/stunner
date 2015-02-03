# stunner
This is just a little repo for some work we did to develop a fix for the "webRTC physical IP address leak bug" thing (https://cryptostorm.org/webrtc), under Windows.

First step was collecting known IP addresses for STUN servers used to establish presence discovery under the webRTC protocol framework, in the Firefox and Chrome universes - that's the two files you'll see with address stuff dumped into them.

Those were de-duped and turned into a little script to block packets going out to those IPs. Thus, no leaked webRTC packets with physical IP in them (for any browsers in those ecosystems).

More detail found in the full write-up, linked above. This is just a place to put stuff, really, so don't get your hopes up :-)


https://twitter.com/cryptostorm_is/status/562324849658720257

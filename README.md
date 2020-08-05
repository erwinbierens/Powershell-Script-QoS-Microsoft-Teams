# Powershell-Script-QoS-Microsoft-Teams
Activate Quality of Service on your (local) Workstation.

This powershell script will setup some QoS rules and will activate QoS via Registry.

It will add the following rules:

Client source port	Protocol	Media category	Common DSCP value	DSCP class
50,000 – 50,019	TCP/UDP	Audio	46	Expedited Forwarding (EF)
50,020 – 50,039	TCP/UDP	Video	34	Assured Forwarding (AF41)
50,040 – 50,059	TCP/UDP	Application/Desktop Sharing and File Transfer	18	Class Selector (CS3)

Make sure the rest of your network is also fully QoS enabled.

# check_ddos
Monitoring of DDoS SYN flood attacks (SYN flood attack) is a type of denial of service or denial of distributed service (DDoS) attack, which consists of direct overhead in the transport layer and indirect in the application layer of the OSI target system model with a sequence of SYN requisitions. Despite the DOS or DDoS attacks do not compromise systems with intrusions or infections with viruses They aim to make services and/or systems unavailable, generating financial losses or reputation damages.

This Nagios plugin monitors system network connections alerting whenever a large number of SYN recv states are verified. The quantities of connections to be considered excessive are passed as arguments, and when Nagios is exceeded alert with the states warning or critical.

Mandatory arguments: The following arguments must be specified when the module is executed:

-w or --warning used to specify the number of connections from which to consider as warning.

-c or --critical used to specify the number of connections from which the result should be considered as critical.

Optional arguments: The following arguments are optionally invoked, as user needs:

-V or --version used to query the module version.

-A or --author used to query the author's data.

Command-Line Execution example

./check_ddos.py -c 300 -w 200


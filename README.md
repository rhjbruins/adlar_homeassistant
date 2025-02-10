The file here are the configuration files to bi-directionally connect Home Assistant to an Adlar / Solareast Heatpump using a modbus TCP connection

Steps in installing are simple, add (and update accordingly!) the 4 files with adlar as a name, and add them to the configuration.yaml, or use the !include options

- the automation takes care of the heat curve select. Use a own risk (i.e. putting >40 C water thru underfloor heating!) Or remove the selection from input select!
- modbus allows for communication with the heatpump (update the IP address and port to suit your config)
- template allows for the translation of bitcode to human readable ON/OFF (only 1 there, defrost)
- input select for the 2 heatcurve selections

NOTE:
- The temperature in the Unit mode is based on the inlet temperature (change to preference)
- For safety not all the codes have been added to prevent doing unwanted things by others (i.e. wife, and backpockets)

References:
- R290 Solareast engineering manual

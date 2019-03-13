# CA-UIM---Mail-Eater
Turns email into UIM events

The file is too big to upload to GitHub, available via link below:

https://drive.google.com/file/d/175vKsMe_MFCB538jqR2RDPuyjXNohr-a/view?usp=sharing

The syntax is:
# gmail2event
 
This tool reads an inbox on a imap compatible mail-server and transforms it into a UIM message
 
Usage: Event

       -endpoint (-e) "imap endpoint"

       -userid (-u) "userid"
       
       -password (-p) "password"
Optional

       -seen - marks the message as read

       -debug

       -UIM - sends the message to UIM event

       -dontdelete (-dd) - do not delete the processed emails

       -snmp (-s) send snmpv1 trap to localhost
 
ie: java -jar C:\tmp\UIM\gmail2event-0.0.1-SNAPSHOT-jar-with-dependencies.jar -debug -p yourpassword -u yourimap@your.domain -e imap.gmail.com -dd -UIM
 
So, you need java on the box (tested with 1.8) and you need a UIM Robot on the box where you run this.
 
Default imap port is used (993), Tested against gmail.

Disclaimer: Not my work.

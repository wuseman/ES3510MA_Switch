# ES3510MA

Lets keep this repo minimal, neat and elegant.

The funny thing is that I got it from a friend a few years ago (my friends are awesome they supporting me alot with all kind of hardware just for fun, you know who you are)

When I'm done with a device I can not see it anymore and 9 out of 10 gadgets end up in the trash NOW value,
for me the knowledge is the all valuable. I do not hack anything for money, everything as a hobbit.

Personally I have a 10Gbit fibre connection + 1Gbit (sorry telia, but there was a port free om the switch)  
and it can only handle 2GBiT but has a transfer speed of 5.6Gb / s, it is damn much better than I thought anyway. 

I was really  surprised when I found it in the box and googled it quickly so I became curious because there is not much info online about it.
Well, the day this repo was created is the day I started playing with this device, so I am completely unaware of what awaits for challenges;)


## How to get started and access: 


- Serial Console (RS-232)

    This port is used to connect a console device to the switch through a serial cable.
    The console device can be a PC or workstation running a VT-100 terminal
    emulator, or a VT-100 terminal. A crossover RJ-45 to DB-9 cable is supplied with
    the unit for connecting to the console port, as illustrated below. The PIN
    assignments used to connect to the serial port are described below.

- Wiring map for serial cable:

    Switch 8-PIN Serial Port Null Modem PC’s 9-PIN DTE Port

        6 RXD (receive data) .......> 3 TXD (transmit data)
        3 TXD (transmit data).......> 2 RXD (receive data)   
        5 SGND (signal ground)......: 5 SGND (signal ground)

- Serial port’s configuration

        Baud Rate..................: 115200 bps
        Character..................: Size—8 Characters
        Data Bits..................: bits—8
        Stop Bits..................: 1
        Flow Control...............: Non
        Parity.....................: /dev/null
        Console Timeout............: 0 (Disabled as default)

- Misc Authentication 

        Privileged Exec Level
        
            Username.....................: admin
            Password.....................: admin

        Normal Exec Level

            Username.....................: guest
            Passowrd.....................: guest

    ,-> Enable Privileged Exec:
    |
    '----> This works from Normal Exec Level only
        
            Password.....................: super

- Authentication Various (Default)

            RADIUS Authentication.......: Disabled
            TACACS+ Authentication......: Disabled
            802.1X Port Authentication..: Disabled
            HTTPS.......................: Enabled
            SSH.........................: Disabled
            Port Security...............: Disabled
            IP Filtering................: Disabled
            DHCP Snooping...............: Disabled


- Telnet

        Telnet ConnectionTelnet operates over the IP transport protocol. 
        In this environment, yourmanagement station and any network device 
        you want to manage over the networkmust have a valid IP address. 

        Valid IP addresses consist of four numbers, 0 to 255,separated by periods. 
        Each address consists of a network portion and host portion.For example, 
        the IP address assigned to this switch, 10.1.0.1, consists 
        of a networkportion (10.1.0) and a host portion.


- Misc Commands in Cli


        enable..................................: Activates privileged mode
        disable.................................: Returns to normal mode from privileged mode
        configure...............................: Activates global configuration mode
        show history............................: Shows the command history buffer
        reload..................................: Restarts the system
        prompt..................................: Customizes the CLI prompt
        end.....................................: Returns to Privileged Exec mode
        exit....................................: Returns to the previous configuration mode, or exits the CLI
        quit....................................: Exits a CLI session
        help....................................: Print help 
        ?.......................................: Print help



## References

    https://www.edge-core.com/_upload/images/ecs3510_28t_v1_5_1_17_bix.zip
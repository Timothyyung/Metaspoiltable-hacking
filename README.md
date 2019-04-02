# Metaspoiltable-hacking

# Created several different virutal machines to run test on.
- Used a software called metapoilatble 2.0 to help demostrate some of the common vunerablitlies in certain systems


# Logs of metasploit

msf > help

Core Commands
=============

    Command       Description
    -------       -----------
    ?             Help menu
    banner        Display an awesome metasploit banner
    cd            Change the current working directory
    color         Toggle color
    connect       Communicate with a host
    exit          Exit the console
    get           Gets the value of a context-specific variable
    getg          Gets the value of a global variable
    grep          Grep the output of another command
    help          Help menu
    history       Show command history
    load          Load a framework plugin
    quit          Exit the console
    repeat        Repeat a list of commands
    route         Route traffic through a session
    save          Saves the active datastores
    sessions      Dump session listings and display information about sessions
    set           Sets a context-specific variable to a value
    setg          Sets a global variable to a value
    sleep         Do nothing for the specified number of seconds
    spool         Write console output into a file as well the screen
    threads       View and manipulate background threads
    unload        Unload a framework plugin
    unset         Unsets one or more context-specific variables
    unsetg        Unsets one or more global variables
    version       Show the framework and console library version numbers


Module Commands
===============

    Command       Description
    -------       -----------
    advanced      Displays advanced options for one or more modules
    back          Move back from the current context
    info          Displays information about one or more modules
    loadpath      Searches for and loads modules from a path
    options       Displays global options or for one or more modules
    popm          Pops the latest module off the stack and makes it active
    previous      Sets the previously loaded module as the current module
    pushm         Pushes the active or list of modules onto the module stack
    reload_all    Reloads all modules from all defined module paths
    search        Searches module names and descriptions
    show          Displays modules of a given type, or all modules
    use           Selects a module by name


Job Commands
============

    Command       Description
    -------       -----------
    handler       Start a payload handler as job
    jobs          Displays and manages jobs
    kill          Kill a job
    rename_job    Rename a job


Resource Script Commands
========================

    Command       Description
    -------       -----------
    makerc        Save commands entered since start to a file
    resource      Run the commands stored in a file


Developer Commands
==================

    Command       Description
    -------       -----------
    edit          Edit the current module or a file with the preferred editor
    irb           Open an interactive Ruby shell in the current context
    log           Display framework.log paged to the end if possible
    pry           Open the Pry debugger on the current module or Framework
    reload_lib    Reload Ruby library files from specified paths


Database Backend Commands
=========================

    Command           Description
    -------           -----------
    db_connect        Connect to an existing database
    db_disconnect     Disconnect from the current database instance
    db_export         Export a file containing the contents of the database
    db_import         Import a scan result file (filetype will be auto-detected)
    db_nmap           Executes nmap and records the output automatically
    db_rebuild_cache  Rebuilds the database-stored module cache
    db_status         Show the current database status
    hosts             List all hosts in the database
    loot              List all loot in the database
    notes             List all notes in the database
    services          List all services in the database
    vulns             List all vulnerabilities in the database
    workspace         Switch between database workspaces


Credentials Backend Commands
============================

    Command       Description
    -------       -----------
    creds         List all credentials in the database

msf > use exploit/windows/
Display all 1045 possibilities? (y or n)
msf > use exploit/windows/smb/ms09_050_smb2_negotiate_func_index 
msf exploit(windows/smb/ms09_050_smb2_negotiate_func_index) > help

Core Commands
=============

    Command       Description
    -------       -----------
    ?             Help menu
    banner        Display an awesome metasploit banner
    cd            Change the current working directory
    color         Toggle color
    connect       Communicate with a host
    exit          Exit the console
    get           Gets the value of a context-specific variable
    getg          Gets the value of a global variable
    grep          Grep the output of another command
    help          Help menu
    history       Show command history
    load          Load a framework plugin
    quit          Exit the console
    repeat        Repeat a list of commands
    route         Route traffic through a session
    save          Saves the active datastores
    sessions      Dump session listings and display information about sessions
    set           Sets a context-specific variable to a value
    setg          Sets a global variable to a value
    sleep         Do nothing for the specified number of seconds
    spool         Write console output into a file as well the screen
    threads       View and manipulate background threads
    unload        Unload a framework plugin
    unset         Unsets one or more context-specific variables
    unsetg        Unsets one or more global variables
    version       Show the framework and console library version numbers


Module Commands
===============

    Command       Description
    -------       -----------
    advanced      Displays advanced options for one or more modules
    back          Move back from the current context
    info          Displays information about one or more modules
    loadpath      Searches for and loads modules from a path
    options       Displays global options or for one or more modules
    popm          Pops the latest module off the stack and makes it active
    previous      Sets the previously loaded module as the current module
    pushm         Pushes the active or list of modules onto the module stack
    reload_all    Reloads all modules from all defined module paths
    search        Searches module names and descriptions
    show          Displays modules of a given type, or all modules
    use           Selects a module by name


Job Commands
============

    Command       Description
    -------       -----------
    handler       Start a payload handler as job
    jobs          Displays and manages jobs
    kill          Kill a job
    rename_job    Rename a job


Resource Script Commands
========================

    Command       Description
    -------       -----------
    makerc        Save commands entered since start to a file
    resource      Run the commands stored in a file


Developer Commands
==================

    Command       Description
    -------       -----------
    edit          Edit the current module or a file with the preferred editor
    irb           Open an interactive Ruby shell in the current context
    log           Display framework.log paged to the end if possible
    pry           Open the Pry debugger on the current module or Framework
    reload_lib    Reload Ruby library files from specified paths


Database Backend Commands
=========================

    Command           Description
    -------           -----------
    db_connect        Connect to an existing database
    db_disconnect     Disconnect from the current database instance
    db_export         Export a file containing the contents of the database
    db_import         Import a scan result file (filetype will be auto-detected)
    db_nmap           Executes nmap and records the output automatically
    db_rebuild_cache  Rebuilds the database-stored module cache
    db_status         Show the current database status
    hosts             List all hosts in the database
    loot              List all loot in the database
    notes             List all notes in the database
    services          List all services in the database
    vulns             List all vulnerabilities in the database
    workspace         Switch between database workspaces


Credentials Backend Commands
============================

    Command       Description
    -------       -----------
    creds         List all credentials in the database


Exploit Commands
================

    Command       Description
    -------       -----------
    check         Check to see if a target is vulnerable
    exploit       Launch an exploit attempt
    rcheck        Reloads the module and checks if the target is vulnerable
    recheck       Alias for rcheck
    reload        Just reloads the module
    rerun         Alias for rexploit
    rexploit      Reloads the module and launches an exploit attempt
    run           Alias for exploit

msf exploit(windows/smb/ms09_050_smb2_negotiate_func_index) > show targets

Exploit targets:

   Id  Name
   --  ----
   0   Windows Vista SP1/SP2 and Server 2008 (x86)


msf exploit(windows/smb/ms09_050_smb2_negotiate_func_index) > show payloads



Compatible Payloads
===================

   Name                                                Disclosure Date  Rank    Description
   ----                                                ---------------  ----    -----------
   generic/custom                                                       normal  Custom Payload
   generic/debug_trap                                                   normal  Generic x86 Debug Trap
   generic/shell_bind_tcp                                               normal  Generic Command Shell, Bind TCP Inline
   generic/shell_reverse_tcp                                            normal  Generic Command Shell, Reverse TCP Inline
   generic/tight_loop                                                   normal  Generic x86 Tight Loop
   windows/adduser                                                      normal  Windows Execute net user /ADD
   windows/dllinject/bind_hidden_ipknock_tcp                            normal  Reflective DLL Injection, Hidden Bind Ipknock TCP Stager
   windows/dllinject/bind_hidden_tcp                                    normal  Reflective DLL Injection, Hidden Bind TCP Stager
   windows/dllinject/bind_ipv6_tcp                                      normal  Reflective DLL Injection, Bind IPv6 TCP Stager (Windows x86)
   windows/dllinject/bind_ipv6_tcp_uuid                                 normal  Reflective DLL Injection, Bind IPv6 TCP Stager with UUID Support (Windows x86)
   windows/dllinject/bind_named_pipe                                    normal  Reflective DLL Injection, Windows x86 Bind Named Pipe Stager
   windows/dllinject/bind_nonx_tcp                                      normal  Reflective DLL Injection, Bind TCP Stager (No NX or Win7)
   windows/dllinject/bind_tcp                                           normal  Reflective DLL Injection, Bind TCP Stager (Windows x86)
   windows/dllinject/bind_tcp_rc4                                       normal  Reflective DLL Injection, Bind TCP Stager (RC4 Stage Encryption, Metasm)
   windows/dllinject/bind_tcp_uuid                                      normal  Reflective DLL Injection, Bind TCP Stager with UUID Support (Windows x86)
   windows/dllinject/reverse_hop_http                                   normal  Reflective DLL Injection, Reverse Hop HTTP/HTTPS Stager
   windows/dllinject/reverse_http                                       normal  Reflective DLL Injection, Windows Reverse HTTP Stager (wininet)
   windows/dllinject/reverse_http_proxy_pstore                          normal  Reflective DLL Injection, Reverse HTTP Stager Proxy
   windows/dllinject/reverse_ipv6_tcp                                   normal  Reflective DLL Injection, Reverse TCP Stager (IPv6)
   windows/dllinject/reverse_nonx_tcp                                   normal  Reflective DLL Injection, Reverse TCP Stager (No NX or Win7)
   windows/dllinject/reverse_ord_tcp                                    normal  Reflective DLL Injection, Reverse Ordinal TCP Stager (No NX or Win7)
   windows/dllinject/reverse_tcp                                        normal  Reflective DLL Injection, Reverse TCP Stager
   windows/dllinject/reverse_tcp_allports                               normal  Reflective DLL Injection, Reverse All-Port TCP Stager
   windows/dllinject/reverse_tcp_dns                                    normal  Reflective DLL Injection, Reverse TCP Stager (DNS)
   windows/dllinject/reverse_tcp_rc4                                    normal  Reflective DLL Injection, Reverse TCP Stager (RC4 Stage Encryption, Metasm)
   windows/dllinject/reverse_tcp_rc4_dns                                normal  Reflective DLL Injection, Reverse TCP Stager (RC4 Stage Encryption DNS, Metasm)
   windows/dllinject/reverse_tcp_uuid                                   normal  Reflective DLL Injection, Reverse TCP Stager with UUID Support
   windows/dllinject/reverse_udp                                        normal  Reflective DLL Injection, Reverse UDP Stager with UUID Support
   windows/dllinject/reverse_winhttp                                    normal  Reflective DLL Injection, Windows Reverse HTTP Stager (winhttp)
   windows/dns_txt_query_exec                                           normal  DNS TXT Record Payload Download and Execution
   windows/download_exec                                                normal  Windows Executable Download (http,https,ftp) and Execute
   windows/exec                                                         normal  Windows Execute Command
   windows/format_all_drives                                            manual  Windows Drive Formatter
   windows/loadlibrary                                                  normal  Windows LoadLibrary Path
   windows/messagebox                                                   normal  Windows MessageBox
   windows/meterpreter/bind_hidden_ipknock_tcp                          normal  Windows Meterpreter (Reflective Injection), Hidden Bind Ipknock TCP Stager
   windows/meterpreter/bind_hidden_tcp                                  normal  Windows Meterpreter (Reflective Injection), Hidden Bind TCP Stager
   windows/meterpreter/bind_ipv6_tcp                                    normal  Windows Meterpreter (Reflective Injection), Bind IPv6 TCP Stager (Windows x86)
   windows/meterpreter/bind_ipv6_tcp_uuid                               normal  Windows Meterpreter (Reflective Injection), Bind IPv6 TCP Stager with UUID Support (Windows x86)
   windows/meterpreter/bind_named_pipe                                  normal  Windows Meterpreter (Reflective Injection), Windows x86 Bind Named Pipe Stager
   windows/meterpreter/bind_nonx_tcp                                    normal  Windows Meterpreter (Reflective Injection), Bind TCP Stager (No NX or Win7)
   windows/meterpreter/bind_tcp                                         normal  Windows Meterpreter (Reflective Injection), Bind TCP Stager (Windows x86)
   windows/meterpreter/bind_tcp_rc4                                     normal  Windows Meterpreter (Reflective Injection), Bind TCP Stager (RC4 Stage Encryption, Metasm)
   windows/meterpreter/bind_tcp_uuid                                    normal  Windows Meterpreter (Reflective Injection), Bind TCP Stager with UUID Support (Windows x86)
   windows/meterpreter/reverse_hop_http                                 normal  Windows Meterpreter (Reflective Injection), Reverse Hop HTTP/HTTPS Stager
   windows/meterpreter/reverse_http                                     normal  Windows Meterpreter (Reflective Injection), Windows Reverse HTTP Stager (wininet)
   windows/meterpreter/reverse_http_proxy_pstore                        normal  Windows Meterpreter (Reflective Injection), Reverse HTTP Stager Proxy
   windows/meterpreter/reverse_https                                    normal  Windows Meterpreter (Reflective Injection), Windows Reverse HTTPS Stager (wininet)
   windows/meterpreter/reverse_https_proxy                              normal  Windows Meterpreter (Reflective Injection), Reverse HTTPS Stager with Support for Custom Proxy
   windows/meterpreter/reverse_ipv6_tcp                                 normal  Windows Meterpreter (Reflective Injection), Reverse TCP Stager (IPv6)
   windows/meterpreter/reverse_named_pipe                               normal  Windows Meterpreter (Reflective Injection), Windows x86 Reverse Named Pipe (SMB) Stager
   windows/meterpreter/reverse_nonx_tcp                                 normal  Windows Meterpreter (Reflective Injection), Reverse TCP Stager (No NX or Win7)
   windows/meterpreter/reverse_ord_tcp                                  normal  Windows Meterpreter (Reflective Injection), Reverse Ordinal TCP Stager (No NX or Win7)
   windows/meterpreter/reverse_tcp                                      normal  Windows Meterpreter (Reflective Injection), Reverse TCP Stager
   windows/meterpreter/reverse_tcp_allports                             normal  Windows Meterpreter (Reflective Injection), Reverse All-Port TCP Stager
   windows/meterpreter/reverse_tcp_dns                                  normal  Windows Meterpreter (Reflective Injection), Reverse TCP Stager (DNS)
   windows/meterpreter/reverse_tcp_rc4                                  normal  Windows Meterpreter (Reflective Injection), Reverse TCP Stager (RC4 Stage Encryption, Metasm)
   windows/meterpreter/reverse_tcp_rc4_dns                              normal  Windows Meterpreter (Reflective Injection), Reverse TCP Stager (RC4 Stage Encryption DNS, Metasm)
   windows/meterpreter/reverse_tcp_uuid                                 normal  Windows Meterpreter (Reflective Injection), Reverse TCP Stager with UUID Support
   windows/meterpreter/reverse_udp                                      normal  Windows Meterpreter (Reflective Injection), Reverse UDP Stager with UUID Support
   windows/meterpreter/reverse_winhttp                                  normal  Windows Meterpreter (Reflective Injection), Windows Reverse HTTP Stager (winhttp)
   windows/meterpreter/reverse_winhttps                                 normal  Windows Meterpreter (Reflective Injection), Windows Reverse HTTPS Stager (winhttp)
   windows/metsvc_bind_tcp                                              normal  Windows Meterpreter Service, Bind TCP
   windows/metsvc_reverse_tcp                                           normal  Windows Meterpreter Service, Reverse TCP Inline
   windows/patchupdllinject/bind_hidden_ipknock_tcp                     normal  Windows Inject DLL, Hidden Bind Ipknock TCP Stager
   windows/patchupdllinject/bind_hidden_tcp                             normal  Windows Inject DLL, Hidden Bind TCP Stager
   windows/patchupdllinject/bind_ipv6_tcp                               normal  Windows Inject DLL, Bind IPv6 TCP Stager (Windows x86)
   windows/patchupdllinject/bind_ipv6_tcp_uuid                          normal  Windows Inject DLL, Bind IPv6 TCP Stager with UUID Support (Windows x86)
   windows/patchupdllinject/bind_named_pipe                             normal  Windows Inject DLL, Windows x86 Bind Named Pipe Stager
   windows/patchupdllinject/bind_nonx_tcp                               normal  Windows Inject DLL, Bind TCP Stager (No NX or Win7)
   windows/patchupdllinject/bind_tcp                                    normal  Windows Inject DLL, Bind TCP Stager (Windows x86)
   windows/patchupdllinject/bind_tcp_rc4                                normal  Windows Inject DLL, Bind TCP Stager (RC4 Stage Encryption, Metasm)
   windows/patchupdllinject/bind_tcp_uuid                               normal  Windows Inject DLL, Bind TCP Stager with UUID Support (Windows x86)
   windows/patchupdllinject/reverse_ipv6_tcp                            normal  Windows Inject DLL, Reverse TCP Stager (IPv6)
   windows/patchupdllinject/reverse_nonx_tcp                            normal  Windows Inject DLL, Reverse TCP Stager (No NX or Win7)
   windows/patchupdllinject/reverse_ord_tcp                             normal  Windows Inject DLL, Reverse Ordinal TCP Stager (No NX or Win7)
   windows/patchupdllinject/reverse_tcp                                 normal  Windows Inject DLL, Reverse TCP Stager
   windows/patchupdllinject/reverse_tcp_allports                        normal  Windows Inject DLL, Reverse All-Port TCP Stager
   windows/patchupdllinject/reverse_tcp_dns                             normal  Windows Inject DLL, Reverse TCP Stager (DNS)
   windows/patchupdllinject/reverse_tcp_rc4                             normal  Windows Inject DLL, Reverse TCP Stager (RC4 Stage Encryption, Metasm)
   windows/patchupdllinject/reverse_tcp_rc4_dns                         normal  Windows Inject DLL, Reverse TCP Stager (RC4 Stage Encryption DNS, Metasm)
   windows/patchupdllinject/reverse_tcp_uuid                            normal  Windows Inject DLL, Reverse TCP Stager with UUID Support
   windows/patchupdllinject/reverse_udp                                 normal  Windows Inject DLL, Reverse UDP Stager with UUID Support
   windows/patchupmeterpreter/bind_hidden_ipknock_tcp                   normal  Windows Meterpreter (skape/jt Injection), Hidden Bind Ipknock TCP Stager
   windows/patchupmeterpreter/bind_hidden_tcp                           normal  Windows Meterpreter (skape/jt Injection), Hidden Bind TCP Stager
   windows/patchupmeterpreter/bind_ipv6_tcp                             normal  Windows Meterpreter (skape/jt Injection), Bind IPv6 TCP Stager (Windows x86)
   windows/patchupmeterpreter/bind_ipv6_tcp_uuid                        normal  Windows Meterpreter (skape/jt Injection), Bind IPv6 TCP Stager with UUID Support (Windows x86)
   windows/patchupmeterpreter/bind_named_pipe                           normal  Windows Meterpreter (skape/jt Injection), Windows x86 Bind Named Pipe Stager
   windows/patchupmeterpreter/bind_nonx_tcp                             normal  Windows Meterpreter (skape/jt Injection), Bind TCP Stager (No NX or Win7)
   windows/patchupmeterpreter/bind_tcp                                  normal  Windows Meterpreter (skape/jt Injection), Bind TCP Stager (Windows x86)
   windows/patchupmeterpreter/bind_tcp_rc4                              normal  Windows Meterpreter (skape/jt Injection), Bind TCP Stager (RC4 Stage Encryption, Metasm)
   windows/patchupmeterpreter/bind_tcp_uuid                             normal  Windows Meterpreter (skape/jt Injection), Bind TCP Stager with UUID Support (Windows x86)
   windows/patchupmeterpreter/reverse_ipv6_tcp                          normal  Windows Meterpreter (skape/jt Injection), Reverse TCP Stager (IPv6)
   windows/patchupmeterpreter/reverse_nonx_tcp                          normal  Windows Meterpreter (skape/jt Injection), Reverse TCP Stager (No NX or Win7)
   windows/patchupmeterpreter/reverse_ord_tcp                           normal  Windows Meterpreter (skape/jt Injection), Reverse Ordinal TCP Stager (No NX or Win7)
   windows/patchupmeterpreter/reverse_tcp                               normal  Windows Meterpreter (skape/jt Injection), Reverse TCP Stager
   windows/patchupmeterpreter/reverse_tcp_allports                      normal  Windows Meterpreter (skape/jt Injection), Reverse All-Port TCP Stager
   windows/patchupmeterpreter/reverse_tcp_dns                           normal  Windows Meterpreter (skape/jt Injection), Reverse TCP Stager (DNS)
   windows/patchupmeterpreter/reverse_tcp_rc4                           normal  Windows Meterpreter (skape/jt Injection), Reverse TCP Stager (RC4 Stage Encryption, Metasm)
   windows/patchupmeterpreter/reverse_tcp_rc4_dns                       normal  Windows Meterpreter (skape/jt Injection), Reverse TCP Stager (RC4 Stage Encryption DNS, Metasm)
   windows/patchupmeterpreter/reverse_tcp_uuid                          normal  Windows Meterpreter (skape/jt Injection), Reverse TCP Stager with UUID Support
   windows/patchupmeterpreter/reverse_udp                               normal  Windows Meterpreter (skape/jt Injection), Reverse UDP Stager with UUID Support
   windows/shell/bind_hidden_ipknock_tcp                                normal  Windows Command Shell, Hidden Bind Ipknock TCP Stager
   windows/shell/bind_hidden_tcp                                        normal  Windows Command Shell, Hidden Bind TCP Stager
   windows/shell/bind_ipv6_tcp                                          normal  Windows Command Shell, Bind IPv6 TCP Stager (Windows x86)
   windows/shell/bind_ipv6_tcp_uuid                                     normal  Windows Command Shell, Bind IPv6 TCP Stager with UUID Support (Windows x86)
   windows/shell/bind_named_pipe                                        normal  Windows Command Shell, Windows x86 Bind Named Pipe Stager
   windows/shell/bind_nonx_tcp                                          normal  Windows Command Shell, Bind TCP Stager (No NX or Win7)
   windows/shell/bind_tcp                                               normal  Windows Command Shell, Bind TCP Stager (Windows x86)
   windows/shell/bind_tcp_rc4                                           normal  Windows Command Shell, Bind TCP Stager (RC4 Stage Encryption, Metasm)
   windows/shell/bind_tcp_uuid                                          normal  Windows Command Shell, Bind TCP Stager with UUID Support (Windows x86)
   windows/shell/reverse_ipv6_tcp                                       normal  Windows Command Shell, Reverse TCP Stager (IPv6)
   windows/shell/reverse_nonx_tcp                                       normal  Windows Command Shell, Reverse TCP Stager (No NX or Win7)
   windows/shell/reverse_ord_tcp                                        normal  Windows Command Shell, Reverse Ordinal TCP Stager (No NX or Win7)
   windows/shell/reverse_tcp                                            normal  Windows Command Shell, Reverse TCP Stager
   windows/shell/reverse_tcp_allports                                   normal  Windows Command Shell, Reverse All-Port TCP Stager
   windows/shell/reverse_tcp_dns                                        normal  Windows Command Shell, Reverse TCP Stager (DNS)
   windows/shell/reverse_tcp_rc4                                        normal  Windows Command Shell, Reverse TCP Stager (RC4 Stage Encryption, Metasm)
   windows/shell/reverse_tcp_rc4_dns                                    normal  Windows Command Shell, Reverse TCP Stager (RC4 Stage Encryption DNS, Metasm)
   windows/shell/reverse_tcp_uuid                                       normal  Windows Command Shell, Reverse TCP Stager with UUID Support
   windows/shell/reverse_udp                                            normal  Windows Command Shell, Reverse UDP Stager with UUID Support
   windows/shell_bind_tcp                                               normal  Windows Command Shell, Bind TCP Inline
   windows/shell_bind_tcp_xpfw                                          normal  Windows Disable Windows ICF, Command Shell, Bind TCP Inline
   windows/shell_hidden_bind_tcp                                        normal  Windows Command Shell, Hidden Bind TCP Inline
   windows/shell_reverse_tcp                                            normal  Windows Command Shell, Reverse TCP Inline
   windows/speak_pwned                                                  normal  Windows Speech API - Say "You Got Pwned!"
   windows/upexec/bind_hidden_ipknock_tcp                               normal  Windows Upload/Execute, Hidden Bind Ipknock TCP Stager
   windows/upexec/bind_hidden_tcp                                       normal  Windows Upload/Execute, Hidden Bind TCP Stager
   windows/upexec/bind_ipv6_tcp                                         normal  Windows Upload/Execute, Bind IPv6 TCP Stager (Windows x86)
   windows/upexec/bind_ipv6_tcp_uuid                                    normal  Windows Upload/Execute, Bind IPv6 TCP Stager with UUID Support (Windows x86)
   windows/upexec/bind_named_pipe                                       normal  Windows Upload/Execute, Windows x86 Bind Named Pipe Stager
   windows/upexec/bind_nonx_tcp                                         normal  Windows Upload/Execute, Bind TCP Stager (No NX or Win7)
   windows/upexec/bind_tcp                                              normal  Windows Upload/Execute, Bind TCP Stager (Windows x86)
   windows/upexec/bind_tcp_rc4                                          normal  Windows Upload/Execute, Bind TCP Stager (RC4 Stage Encryption, Metasm)
   windows/upexec/bind_tcp_uuid                                         normal  Windows Upload/Execute, Bind TCP Stager with UUID Support (Windows x86)
   windows/upexec/reverse_ipv6_tcp                                      normal  Windows Upload/Execute, Reverse TCP Stager (IPv6)
   windows/upexec/reverse_nonx_tcp                                      normal  Windows Upload/Execute, Reverse TCP Stager (No NX or Win7)
   windows/upexec/reverse_ord_tcp                                       normal  Windows Upload/Execute, Reverse Ordinal TCP Stager (No NX or Win7)
   windows/upexec/reverse_tcp                                           normal  Windows Upload/Execute, Reverse TCP Stager
   windows/upexec/reverse_tcp_allports                                  normal  Windows Upload/Execute, Reverse All-Port TCP Stager
   windows/upexec/reverse_tcp_dns                                       normal  Windows Upload/Execute, Reverse TCP Stager (DNS)
   windows/upexec/reverse_tcp_rc4                                       normal  Windows Upload/Execute, Reverse TCP Stager (RC4 Stage Encryption, Metasm)
   windows/upexec/reverse_tcp_rc4_dns                                   normal  Windows Upload/Execute, Reverse TCP Stager (RC4 Stage Encryption DNS, Metasm)
   windows/upexec/reverse_tcp_uuid                                      normal  Windows Upload/Execute, Reverse TCP Stager with UUID Support
   windows/upexec/reverse_udp                                           normal  Windows Upload/Execute, Reverse UDP Stager with UUID Support
   windows/vncinject/bind_hidden_ipknock_tcp                            normal  VNC Server (Reflective Injection), Hidden Bind Ipknock TCP Stager
   windows/vncinject/bind_hidden_tcp                                    normal  VNC Server (Reflective Injection), Hidden Bind TCP Stager
   windows/vncinject/bind_ipv6_tcp                                      normal  VNC Server (Reflective Injection), Bind IPv6 TCP Stager (Windows x86)
   windows/vncinject/bind_ipv6_tcp_uuid                                 normal  VNC Server (Reflective Injection), Bind IPv6 TCP Stager with UUID Support (Windows x86)
   windows/vncinject/bind_named_pipe                                    normal  VNC Server (Reflective Injection), Windows x86 Bind Named Pipe Stager
   windows/vncinject/bind_nonx_tcp                                      normal  VNC Server (Reflective Injection), Bind TCP Stager (No NX or Win7)
   windows/vncinject/bind_tcp                                           normal  VNC Server (Reflective Injection), Bind TCP Stager (Windows x86)
   windows/vncinject/bind_tcp_rc4                                       normal  VNC Server (Reflective Injection), Bind TCP Stager (RC4 Stage Encryption, Metasm)
   windows/vncinject/bind_tcp_uuid                                      normal  VNC Server (Reflective Injection), Bind TCP Stager with UUID Support (Windows x86)
   windows/vncinject/reverse_hop_http                                   normal  VNC Server (Reflective Injection), Reverse Hop HTTP/HTTPS Stager
   windows/vncinject/reverse_http                                       normal  VNC Server (Reflective Injection), Windows Reverse HTTP Stager (wininet)
   windows/vncinject/reverse_http_proxy_pstore                          normal  VNC Server (Reflective Injection), Reverse HTTP Stager Proxy
   windows/vncinject/reverse_ipv6_tcp                                   normal  VNC Server (Reflective Injection), Reverse TCP Stager (IPv6)
   windows/vncinject/reverse_nonx_tcp                                   normal  VNC Server (Reflective Injection), Reverse TCP Stager (No NX or Win7)
   windows/vncinject/reverse_ord_tcp                                    normal  VNC Server (Reflective Injection), Reverse Ordinal TCP Stager (No NX or Win7)
   windows/vncinject/reverse_tcp                                        normal  VNC Server (Reflective Injection), Reverse TCP Stager
   windows/vncinject/reverse_tcp_allports                               normal  VNC Server (Reflective Injection), Reverse All-Port TCP Stager
   windows/vncinject/reverse_tcp_dns                                    normal  VNC Server (Reflective Injection), Reverse TCP Stager (DNS)
   windows/vncinject/reverse_tcp_rc4                                    normal  VNC Server (Reflective Injection), Reverse TCP Stager (RC4 Stage Encryption, Metasm)
   windows/vncinject/reverse_tcp_rc4_dns                                normal  VNC Server (Reflective Injection), Reverse TCP Stager (RC4 Stage Encryption DNS, Metasm)
   windows/vncinject/reverse_tcp_uuid                                   normal  VNC Server (Reflective Injection), Reverse TCP Stager with UUID Support
   windows/vncinject/reverse_udp                                        normal  VNC Server (Reflective Injection), Reverse UDP Stager with UUID Support
   windows/vncinject/reverse_winhttp                                    normal  VNC Server (Reflective Injection), Windows Reverse HTTP Stager (winhttp)

msf exploit(windows/smb/ms09_050_smb2_negotiate_func_index) > 
msf exploit(windows/smb/ms09_050_smb2_negotiate_func_index) > 
msf exploit(windows/smb/ms09_050_smb2_negotiate_func_index) > show options

Module options (exploit/windows/smb/ms09_050_smb2_negotiate_func_index):

   Name   Current Setting  Required  Description
   ----   ---------------  --------  -----------
   RHOST                   yes       The target address
   RPORT  445              yes       The target port (TCP)
   WAIT   180              yes       The number of seconds to wait for the attack to complete.


Exploit target:

   Id  Name
   --  ----
   0   Windows Vista SP1/SP2 and Server 2008 (x86)


msf exploit(windows/smb/ms09_050_smb2_negotiate_func_index) > show advanced

Module advanced options (exploit/windows/smb/ms09_050_smb2_negotiate_func_index):

   Name                    Current Setting    Required  Description
   ----                    ---------------    --------  -----------
   CHOST                                      no        The local client address
   CPORT                                      no        The local client port
   ConnectTimeout          10                 yes       Maximum number of seconds to establish a TCP connection
   ContextInformationFile                     no        The information file that contains context information
   DisablePayloadHandler   false              no        Disable the handler code for the selected payload
   EnableContextEncoding   false              no        Use transient context when encoding payloads
   NTLM::SendLM            true               yes       Always send the LANMAN response (except when NTLMv2_session is specified)
   NTLM::SendNTLM          true               yes       Activate the 'Negotiate NTLM key' flag, indicating the use of NTLM responses
   NTLM::SendSPN           true               yes       Send an avp of type SPN in the ntlmv2 client blob, this allows authentication on Windows 7+/Server 2008 R2+ when SPN is required
   NTLM::UseLMKey          false              yes       Activate the 'Negotiate Lan Manager Key' flag, using the LM key when the LM response is sent
   NTLM::UseNTLM2_session  true               yes       Activate the 'Negotiate NTLM2 key' flag, forcing the use of a NTLMv2_session
   NTLM::UseNTLMv2         true               yes       Use NTLMv2 instead of NTLM2_session when 'Negotiate NTLM2' key is true
   Proxies                                    no        A proxy chain of format type:host:port[,type:host:port][...]
   SMB::ChunkSize          500                yes       The chunk size for SMB segments, bigger values will increase speed but break NT 4.0 and SMB signing
   SMB::Native_LM          Windows 2000 5.0   yes       The Native LM to send during authentication
   SMB::Native_OS          Windows 2000 2195  yes       The Native OS to send during authentication
   SMB::VerifySignature    false              yes       Enforces client-side verification of server response signatures
   SMBDirect               true               no        The target port is a raw SMB service (not NetBIOS)
   SMBDomain               .                  no        The Windows domain to use for authentication
   SMBName                 *SMBSERVER         yes       The NetBIOS hostname (required for port 139 connections)
   SMBPass                                    no        The password for the specified username
   SMBUser                                    no        The username to authenticate as
   SSL                     false              no        Negotiate SSL/TLS for outgoing connections
   SSLCipher                                  no        String for SSL cipher - "DHE-RSA-AES256-SHA" or "ADH"
   SSLVerifyMode           PEER               no        SSL verification method (Accepted: CLIENT_ONCE, FAIL_IF_NO_PEER_CERT, NONE, PEER)
   SSLVersion              Auto               yes       Specify the version of SSL/TLS to be used (Auto, TLS and SSL23 are auto-negotiate) (Accepted: Auto, TLS, SSL23, SSL3, TLS1, TLS1.1, TLS1.2)
   VERBOSE                 false              no        Enable detailed status messages
   WORKSPACE                                  no        Specify the workspace for this module
   WfsDelay                0                  no        Additional delay when waiting for a session

msf exploit(windows/smb/ms09_050_smb2_negotiate_func_index) > show evasion

Module evasion options:

   Name                           Current Setting  Required  Description
   ----                           ---------------  --------  -----------
   SMB::obscure_trans_pipe_level  0                yes       Obscure PIPE string in TransNamedPipe (level 0-3)
   SMB::pad_data_level            0                yes       Place extra padding between headers and data (level 0-3)
   SMB::pad_file_level            0                yes       Obscure path names used in open/create (level 0-3)
   SMB::pipe_evasion              false            yes       Enable segmented read/writes for SMB Pipes
   SMB::pipe_read_max_size        1024             yes       Maximum buffer size for pipe reads
   SMB::pipe_read_min_size        1                yes       Minimum buffer size for pipe reads
   SMB::pipe_write_max_size       1024             yes       Maximum buffer size for pipe writes
   SMB::pipe_write_min_size       1                yes       Minimum buffer size for pipe writes
   TCP::max_send_size             0                no        Maxiumum tcp segment size.  (0 = disable)
   TCP::send_delay                0                no        Delays inserted before every send.  (0 = disable)

msf exploit(windows/smb/ms09_050_smb2_negotiate_func_index) > back
msf > ls
[*] exec: ls

Documents
fakeuname.c
pi-bluetooth+re4son_2.2_all.deb
scripts
Wormy
msf > search portscan
[!] Module database cache not built yet, using slow search


Matching Modules
================

   Name                                              Disclosure Date  Rank    Description
   ----                                              ---------------  ----    -----------
   auxiliary/scanner/http/wordpress_pingback_access                   normal  Wordpress Pingback Locator
   auxiliary/scanner/natpmp/natpmp_portscan                           normal  NAT-PMP External Port Scanner
   auxiliary/scanner/portscan/ack                                     normal  TCP ACK Firewall Scanner
   auxiliary/scanner/portscan/ftpbounce                               normal  FTP Bounce Port Scanner
   auxiliary/scanner/portscan/syn                                     normal  TCP SYN Port Scanner
   auxiliary/scanner/portscan/tcp                                     normal  TCP Port Scanner
   auxiliary/scanner/portscan/xmas                                    normal  TCP "XMas" Port Scanner
   auxiliary/scanner/sap/sap_router_portscanner                       normal  SAPRouter Port Scanner
:

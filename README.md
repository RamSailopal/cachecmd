
AUTHOR - Raman Sailopal

BACKGROUND - Simple command line utility to interface with Intersystems IRIS environment via an IRIS session

USAGE 

    - Parameter 1 - The namespace
     
      Parameter 2 - The objectscript command
      
  example 1:

     cachecmd "USER" 'S ^TEST("TEST")="TEST"'

This will set up a global TEST with a subscript TEST and a value TEST, on an instance named IRIS and in the USER namespace

  example 2:
     
     cachecmd "USER" 'W ^TEST("TEST")'
     TEST

This will return the TEST value created in example 1

PREREQUISITES 
    
      - An installed version of intersystems IRIS (See iris repo for installation with Ansible)
              
      - grep installed on the machine running iriscmd

INSTALLATION - Run:

      git clone https://github.com/RamSailopal/cachecmd.git
      mv iriscmd/cachecmd /usr/local/bin 	

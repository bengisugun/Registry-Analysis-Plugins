# Registry Analysis Plugins

1)hivelist: Find and list available registry hives.

    Example: vol.py hivelist
  
  This command allows users to find and display a list of the available registry hives, which are files that contain the data stored in the registry.

2)hivedump: Print all keys and subkeys in a hive.
    
    Example: vol.py hivedump –o 0xe1a14b60
  
  This command allows users to print out all of the keys and subkeys in a specific registry hive. The -o flag specifies the offset of the hive to dump, which is the virtual address where the hive is stored in memory.

3)printkey: Output a registry key, subkeys, and values.
    
     Example: vol.py printkey –K "Microsoft\Windows\CurrentVersion\Run"
  
  This command allows users to output a specific registry key, along with its subkeys and values. The -K flag specifies the path of the key to output.


4)dumpregistry: Extract all available registry hives.
   
     Example: vol.py dumpregistry --dump-dir ./output
  
  This command allows users to extract all available registry hives and save them to a specified directory. The -o flag specifies the virtual offset of the hive to extract, and the --dump-dir flag specifies the directory to save the extracted files.

5)userassist: Find and parse userassist key values.
   
    Example: vol.py userassist
  
  This command allows users to find and parse the values of the userassist key in the registry, which stores information about programs that are automatically run when a user logs in.


6)hashdump: Dump user NTLM and Lanman hashes.
    
    Example: vol.py hashdump
  
  This command allows users to dump the NTLM and Lanman hashes of user accounts, which can be used to crack passwords.

7)autoruns: Map ASEPs to running processes.
    
    Example: vol.py autoruns -v
  
  This command allows users to map Autostart Extensibility Points (ASEPs) to running processes, which can be used to identify programs that are automatically started when the system boots up. The -v flag specifies that the command should show everything.

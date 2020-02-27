# portScanner

Usage: sudo portScanner -H <target host> -p <target port> {-t|-u|-r}

Options:

  -h, --help  show this help message and exit
  
  -H TGTHOST  specify target host
  
  -p TGTPORT  specify target port[s] separated by comma
  
  -u          Scan UDP connections
  
  -t          Scan TCP connections
  
  -r          Use range of ports instead of specific ports. Separated by "-"
  
  
  
  Example: 
  
  01. Scan TCP connections for ports 21, 23 and 40, on target 192.168.43.248:
  
    sudo ./portScanner -H 192.168.43.248 -p "21, 23, 40" -t
      
  
  02. Scan UDP connections for ports 100 to 120, on target 192.168.43.248:
  
    sudo ./portScanner -H 192.168.43.248 -p "100-120" -u -r
      
      

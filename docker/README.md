# About Docker For Samba

### Notice
  1. In this section, the defautl 'docker run' command does not use port parameter which to use for sending log infor.

  ```
    # Expose log port:
    
    docker run -p 514:514 -p 514:514/udp -p 137:137/udp -p 138:138/udp -p 139:139 -p 445:445 -ti -v /home/tmp/:/srv/samba/backup/ 971985ff7fb8 -n -u "abc:123456"
    
    # Port 514 is the default log port for rsyslogd
  ```
  
  2. If you want to run it with 'background' mode, you have to add '**-d**' in docker command line.

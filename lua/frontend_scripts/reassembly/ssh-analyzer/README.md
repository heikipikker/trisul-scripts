ssh passive analysis
====================


Uses the techniques described in [Traffic Analysis of Secure Shell ](http://localhost:3000/blog/analysing-ssh/post.html)  to

1. detect successful logins
2. detect keystrokes after a successful login
3. detect SSH Tunnels,  forward or reverse


The files are
- ssh_dissect.lua  -- SSH protocol analyzer 
- ssh-spy.lua -- connects the ssh_dissect.lua into Trisul TCP Reassembly 
- ssh-alert-group.lua -- a new alert group to house the alerts 


The scripts uses the `PDURecord` and `SweepBuffer` helpers from the BitMaul library.



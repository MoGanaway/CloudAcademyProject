# Documentation for CLoud Academy Project : #
## Steps ##
1.  Open GCP using Qwiklabs
2.  Go to Firewall --> VPC Network--> Add Firewall  rule
3.  Name it http-https-AllowSecurityGaurd
4.  Go to Target --> Choose "*allow all instances in the network*"
5.  Go to Sources --> Type "*0,0,0,0/0*" to choose all the sources
6.  Go to *Protocols & Ports* --> *Specified Protocols & Ports*
7.  Check the TCP box.
8.  Type "*80, 8080, 443*" in the Ports bar.
9.  Go to *Compute Engine* --> Create an istance with the specified attributes.
10. Go to *VM Instances* --> find the instance you previuosly made.
11. Press on **SSH** to use the command line.
12. Type "*sudo apt-get update -y*"
13. Type "*sudo apt-get install apache2 -y*"
14. Make sure the web server works using the external IP address.
15. Go back to the **SSH** and Type "*cd /var/www/html/*"
16. Then type "*ls*" to see what files are in this directory --> you will find '*index.html*'
17. Upload your own index.html file using the arrow In the top right, it will be saved in /home/$ USER $/ 
18. Then type "*sudo cp /home/$ USER $/myindex.html /var/www/html/index.html*" to replace the index.html in /var/www.html/ with your own myindex.html

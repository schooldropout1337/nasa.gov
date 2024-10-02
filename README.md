![spongematrix](https://github.com/schooldropout1337/nasa.gov/blob/main/nasa-gov-spongematrix.jpg)

# nasa.gov
Subdomain, Hostname, IP and Security Research on NASA.GOV

# nasa-alive.txt
656 live subdomains - lots more to probe. 

# httpx (probe more subdomains)
httpx -l nasa.txt -p 80,443,8080,8443,3128 -mc 200,301,302,401 -o nasa-alive-2nd.txt -resume resume.cfg

# nuclei template - reflection.yaml
nuclei -t reflection.yaml -l nasa-alive.txt

![reflection](https://github.com/schooldropout1337/nasa.gov/blob/main/nasa-gov.jpg)

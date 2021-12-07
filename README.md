# Honeypot Assignment

**Time spent:** **4** hours spent in total

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.

### MHN-Admin Deployment (Required)

**Summary:** I decided to follow the guide and use gcloud to implement the virtual machines. It was nice to learn a little about how to use gcloud as it is something I have never used before. It was a little difficult at first, but once I understood the way gcloud is laid out, it was pretty simple.

<img src="mhn-admin.gif">

### Dionaea Honeypot Deployment (Required)

**Summary:** Dionaea is a honeypot that focusses on capturing the type of attacks as well as the signatures of malware those attacks attempt to use, if any.

<img src="dionaea-honeypot.gif">

### Database Backup (Required) 

**Summary:** MHN uses MongoDB as its RDBMS system. The exported json file contains all the information from the attacks captured by the honeypots.

*Be sure to upload session.json directly to this GitHub repo/branch in order to get full credit.*

### Deploying Additional Honeypot(s) (Optional)

#### Snort Honeypot

**Summary:** Snort is a simple honeypot that captures traffic of incoming IP's that behave maliciously.

<img src="x-honeypot.gif">

### Malware Capture and Identification (Optional)

#### X Malware

**Summary:** This malware was captured by the Dionaea Honeypot. When put through the VirusTotal search engine, it was identified as the WannaCry ransomeware. This malware actually appeared quite often in my Dionaea captures.

MD5 Hash: 6e72ad805b4322612b9c9c7673a45635

<img src="x-malware.gif">

## Notes

I had a lot of trouble understanding how to use gcloud at first, but eventually I understood how it all fit together and it was actually pretty easy to use. It was really frightening how fast attacks started appearing. I think there were more than 50 in the first 5 minutes. Also, at one point, my honeypot machines stopped communicating with the MHN-Admin machine, so I had to redo the setup, but thankfully it was pretty quick.

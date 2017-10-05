# AutoBlockIPs
AutoBlock IPs that do a dictionary attack on your SSH server

Have you ever noticed that the sshd on your publicly facing machines gets bombarded with dictionary attacks several times per day? This problem is mostly an annoyance, as it fills up the logs with lots of User authentication failed, wrong password for <username> messages. There are of course several ways to work around this problem, and the most common one is to run sshd on another port than 22. I find that approach cumbersome, because it means you'll always have to configure your client software to connect to a non-standard port, and in lots of cases a firewall at your location might be blocking the traffic as well. Isn't there a way to block these bothersome users instead?


SafeHaven Portal is a secure and innovative platform that enables citizens to report illegal activities, suspicious behavior, or neglected areas needing law enforcement attention. Designed to promote a public-social partnership, the portal creates a bridge between society and law enforcement agencies (LEAs), making communities safer and fostering trust.
The platform uses OTP-based login which can be traced back to Aadhaar for secure access and allows users to submit complaints anonymously, ensuring their privacy and encouraging whistleblowers. Complaints are processed using LLM to categorize and prioritize them based on severity, enabling LEAs to focus on high-risk and critical issues efficiently. Geolocation tagging ensures accurate reporting of incidents, while a dedicated LEA dashboard facilitates streamlined complaint management and response.
To maintain accountability, users receive updates on their complaints' status, promoting transparency. A strike system discourages misuse by penalizing users who abuse the platform, including account suspension or bans for repeated offenses. The platform also incorporates a reward mechanism to incentivize actionable and meaningful reports, fostering a proactive approach among users.
By empowering citizens to play an active role in public safety and providing LEAs with actionable insights, SafeHaven addresses critical gaps in law enforcement coverage. It not only helps deter illegal activities but also strengthens the relationship between communities and LEAs. This transformative initiative leverages technology to create a safer society, where every voice can contribute to meaningful change and enhanced security. SafeHaven is the future of collaborative public safety.

Backend user roles and its corresponding privileges
User
/me -> Details about self [ stats ]
/login -> Login with phone number
/otp-verify -> verify page of login
/see-map -> See the heatmap of the place 
/report -> To report an activity 
/report-{id} -> To see status of the report also to provide additional details
/rewards ->  Amount that is to be rewarded to the user for his contribution
/redeem-reward -> External site [Not going to develop]
LEA
/me -> Details about self [ stats ]
/login -> Login with phone number
/otp-verify -> verify page of login
/see-map -> See the heatmap of the place 
/report -> To report an activity 
/report-{id} -> To see status of the report also to provide additional details
                     -> Change status, Add details
                      -> Assign a team, send email
/issue-reward -> To send a reward against a report id
/reward-allocation -> See rewards allocated and rest for the LEA agency
Admin
Will be set up using flask-admin. The page will contain all the reports and activities, will be similar to LEA, but have more abilities like strike off LEA and users, ban phone numbers etc
Frontend
A simple, clean and beautiful UI from bootstrap will be used, the frontend page can either be based on reactjs or vanilla JS, the dependency should be kept simple, Integrating playback for video, Image and Audio is something that will need support of big guns

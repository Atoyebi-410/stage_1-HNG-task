# Linux User Creation Bash Script

### Task

Your company has employed many new developers. As a SysOps engineer, write a bash script called create_users.sh that reads a text file containing the employee’s usernames and group names, where each line is formatted as user;groups.

The script should create users and groups as specified, set up home directories with appropriate permissions and ownership, generate random passwords for the users, and log all actions to /var/log/user_management.log. Additionally, store the generated passwords securely in /var/secure/user_passwords.txt.

Ensure error handling for scenarios like existing users and provide clear documentation and comments within the script.

Also write a technical article explaining your script, linking back to HNG

### Requirements:

 Each User must have a personal group with the same group name as the username, this group name will not be written in the text file.
 A user can have multiple groups, each group delimited by comma ","
 Usernames and user groups are separated by semicolon ";"- Ignore whitespace
e.g.
 light; sudo,dev,www-data
 idimma; sudo
 mayowa; dev,www-data
For the first line, light is username and groups are sudo, dev, www-data
 
### Technical Article: 

The article should be well-structured.
 It MUST include at least two links to the HNG Internship websites; choose from any of https://hng.tech/internship, https://hng.tech/hire, or https://hng.tech/premium so others can learn more about the program.
 The report should be concise.
 The article should be public and accessible by anyone on the internet.

### Acceptance Criteria:

 Successful Run: The mentors will test your script by supplying the name of the text file containing usernames and groups as the first argument to your script (i.e bash create_user.sh <name-of-text-file> ) in an Ubuntu machine.
 All users should be created and assigned to their groups appropriately
 The file /var/log/user_management.log should be created and contain a log of all actions performed by your script.
 The file /var/secure/user_passwords.csv should be created and contain a list of all users and their passwords delimited by comma, and only the file owner should be able to read it.
 The technical article is clear, concise and captures the reasoning behind each step in your script.

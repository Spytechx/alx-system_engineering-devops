su betty				-	Switches Current User to betty
whoami					-	Prints Effective Username
groups					-	prints all the groups of the current user
chown betty hello			-	changes owner of file
touch hello				-	Creates empty file
chmod u+x hello				-	Execution power to owner
chmod ug+x,o+r hello			- 	Execution power to owner and grour and read only power to others
chmod udo+x hello			-	Execution power to all
chmod 007 hello				-	complete read, write, execute power to file
chmod 753 hello				-	setting mode
chmod --reference=olleh hello		-	copying directory privileges
chmod -R +X .				-	execute permission to all subdirectories
mkdir -m 751 my_dir			-	create a directory with permission stated
chgrp school hello			-	changing group owner
chown vincent:school *			-	changing owner and group to a specific owner and group
chown -h vincent:staff _hello		-	changing ownership of file and group owner
chown --from=guillaume betty hello	-	Chaning file owner with conditions if it belongs to a particular user
telenet towel.blinkenlights.nl		-	Playing Star Wars in Terminal

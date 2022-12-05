Shell Redirections

Prints Hello World:	echo -e "Hello, World"

Prints Confused Smiley:	echo "\"(Ôo)'"

Displays a file:	cat /etc/passwd

Displays last 10 lines :	tail /etc/passwd

Displays first 10 lines : 	head /etc/passwd

Displays thrid line of the file iacta :	head --lines=3 iacta | tail --lines=1

Creates an exact file with a name : echo -e "Best School" >> "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)"

Writes into a file : 	ls -la >> ls_cwd_content

Duplicates last line : 	tail -1 iacta >> iacta

Script deletes all regular files with an extension :	find . -name "*.js" -type f -delete

Script that counts the no of directories and sub-directories : find . -mindepth 1 -type d| wc -l

Script displays 10 newest files : 	ls -t1 | head -n 10

Script takes a list of wordsand prints word that apprear once : 	sort | uniq -u

Displays lines containing root pattern : grep -i "root" /etc/passwd

Displays no of line that contain pattern 'bin' :	grep -c -i "bin" /etc/passwd

Displays line containing pattern root and 3 lines after them :	grep -i "root" -A 3 /etc/passwd

Displays line in a file that doesn't contain bin : 	grep -i -v "bin" /etc/passwd

DIsplay lines that mstarts with letter :	grep -i "^[a-z]" /etc/ssh/sshd_config 

replace characters from input :		tr "A" "Z" | tr "c" "e"

removes particular letters from input : 	tr -d "cC"

script reverese input :		rev

Display sorted all users and their home directories : 		cut -d ':' -f 1,6 /etc/passwd | sort

Finds all empty files in current directories and sub-directories :	find . -empty -printf %f'\n'

List all type of a particular file :	find . -type f -name "*.gif" | rev | cut -d'/' -f1 | cut -d'.' -f2,3 | rev | sort -Vf

Script decodes acrostics :	echo "$(cut -c 1 | tr -d '\n')"

Script parses web serves logs in TSV formats:		tail -n +2 | cut -f 1 | sort | uniq -c | sort -nr | head -11 | cut -c 9-

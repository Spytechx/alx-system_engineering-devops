SHELL, INIT FILES, VARIABLES and EXPANSIONS
Creates an ALias:		alias ls="rm *"

Prints Hello user:		echo "hello $USER"

Adds action to PAth:		export PATH=$PATH:/action

Script Counts number of directories in the path:		echo $((`echo $PATH | grep -o ":/" | wc -l`+ 1))

Script lists environment variables :		printenv

Script lists local and environment variables: 		set

CReates new local variable:		BEST="School"

CReates global variables:		export BEST="School"

Prints result of addition of a no with a value stored in a vairable:		echo -e $((128 + TRUEKNOWLEDGE))

Prints result of division of two variables :		echo $(($POWER / $DIVIDE))

Prints result of a vriable to the power of another : 		echo $(($BREATH**$LOVE))

Scripts convets base 2 number to base 10 number:		echo $((2#$BINARY))

Script prints all possible combiantions of two letters except oo:		echo {a..z}{a..z} | tr " " "\n" | grep -v "oo"

script prints a 2 decimal place number:		printf "%.2f" $NUM | sort

Script converts base 10 to base 16 :		printf '%x\n' $DECIMAL

Script encodes and decodes text using rot13 encryption:		tr `echo {a..z} | tr -d ' '` `echo {n..z} $(echo {a..m}) | tr -d ' '` | tr `echo {A..Z} | tr -d ' '` `echo {N..Z} $(echo {A..M}) | tr -d ' '`

Script prints every other line from input:		perl -lne 'print if $. % 2 == 1'

Script add 2 numbers stored in environmen variables and prints result:		echo $(printf %o $(($((5#$(echo $WATER | tr 'water' '01234'))) + $((5#$(echo $STIR | tr 'stir.' '01234'))))) | tr '01234567' 'bestchol')

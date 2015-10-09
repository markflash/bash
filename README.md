# Bash Recipes
This repo contains simple one liner Bash commands that can save your life.

### Recipe 1
Create multiple recursive directories:

```shell
mkdir -p {2000..2015}/{01..12}
```


### Recipe 2
Improvised crossword solutions

*Linux systems contain dictionaries.(On Ubuntu Linux, the path is /usr/share/dict/)
**grep* can be use regular expressions and filter words in these dictionaries to solve crosswords!


e.g.

1. A seven letter word that starts with "e" and ends with "nd".

	```shell
	grep -i '^e....nd$' american-english
	```
2. A nine letter word whose first letter is "d" and sixth letter is "r".
	
	```shell
	grep -i '^[a-z]....r..[a-z]$' american-english
	```

3. A ten letter word that has "r" and "t" as the third and fourth letter respectively.
	```shell
	grep -i '^[a-z].rt.....[a-z]$' american-english 
	```
	
# References

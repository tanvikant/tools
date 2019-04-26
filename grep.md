### Grep a file but show surrounding lines for context

grep -B3 -A2 foo README.txt

### If you want the same number of lines before and after you can use -C num.

grep -C 3 foo README.txt

### Find string while knowing a substring of it.

Sample : The id for the request is entity[123]
grep 'The id for the request is entity' | grep -o 'entity[^[:blank:]]*'


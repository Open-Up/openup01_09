# Open Up! mid term exam correction

## Unix commands

 -Question 1 :

```
find * -name "*.html" -exec sed -i -e 's/3.0.0-beta5/3.0.0-beta6/g' {} \;
```

 -Question 2 : 

```
benwa@horizon ~/Documents/linagora/open-up/s01/e08 (git)-[master] % wc * -l |tail -n 1 | tr -s ' ' | cut -d ' ' -f 2
36
```

## Scripting

 - Question 1 : 

```
#!/bin/bash

mkdir java
mkdir c_plus_plus
```

 - Question 2 :


```
#!/bin/bash

mkdir java || true
mkdir c_plus_plus || true
```

 - Question 3 : 

```
#!/bin/bash

function classify {
  mkdir -p $1

  grep -l $1 * > tmp.txt 

  while read p; do
    mv $p $1
  done <tmp.txt

  rm tmp.txt || true
}

classify java
classify c_plus_plus
```

 - Question 4 : 

```
#!/bin/bash

function classify {
  mkdir -p $1

  if [ "$1" == "-R" ]; then
    grep -r -l $1 * > tmp.txt 
  else
    grep -l $1 * > tmp.txt 
  fi

  while read p; do
    mv $p $1
  done <tmp.txt

  rm tmp.txt || true
}

classify java
classify c_plus_plus

```

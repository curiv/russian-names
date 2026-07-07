How to generate a wordlist

```
#!/bin/bash
prefixes=(a b c d e f g h i j k l m n o p q r s  t u w x y z)

while IFS= read -r surname; do
  for prefix in "${prefixes[@]}"; do
    echo "${surname}_${prefix}"
  done
done < russian_lastnames.txt
```

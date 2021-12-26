


```curl $URL || jq '.[2]| map ([{type:.[0]} , (.[1] | map({(.[0]):(.[3]) }) | add)] | add) | sort_by(.dtstart)' > data/Calendar.json```

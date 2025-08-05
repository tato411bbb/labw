# labw
lab2
Build own perplexity https://dev.to/shayy/how-to-build-a-perplexity-clone-ai-search-engine-with-ai-agents-28g1


#!/bin/bash

PATH=/sbin:/usr/sbin:/bin:/usr/bin

cd /var/www/html/4up

kjr=$(/usr/bin/find /var/www/html/4up -type f -exec stat -c '%Y %n' {} \; | sort -nr | head -n1 | cut -d' ' -f2-)

DIR="/var/www/html/4up"
FILE="$kjr"

# Loop through all files in the directory
for item in "$DIR"/*; do
    # If the current item is not the desired file, remove it
    if [ "$item" != "$FILE" ]; then
        rm -fr  "$item"
    fi
done







echo $kjr



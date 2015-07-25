#!/bin/bash
COMMAND=$1
FILE=$2
NOTE_DIR="/etc/note/"
if [ -z ${COMMAND} ];
then
        echo "ERROR: Command is missing";
        exit
fi
if [ -z ${FILE} ];
then
        echo "ERROR: File is missing";
        exit
fi
if [ "$COMMAND" == "set" ]; then
        NOTE=$3
        echo "$NOTE" > "$NOTE_DIR/$FILE"
fi
if [ "$COMMAND" == "read" ]; then
        cat "$NOTE_DIR/$FILE"
fi

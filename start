#!/bin/bash

# Start the first process
gunicorn app:app &

# Start the second process
python3 bot.py &

# Wait for any process to exit
wait -n

# Exit with status of process that exited first
exit $?

# Dockerfile Bug: Missing Dependencies and Incorrect CMD

This repository demonstrates a common error in Dockerfiles: failure to install required packages and incorrect usage of the CMD instruction. The original Dockerfile attempts to run a Python web server without installing necessary dependencies and utilizes an inefficient `CMD` instruction.

The solution involves adding a `requirements.txt` file and correcting the `CMD` instruction for optimal execution.

## Bug

The provided `Dockerfile` attempts to run a Python web server without specifying its dependencies, leading to a runtime error. The `CMD` instruction is also not optimized. 

## Solution

The solution includes adding a `requirements.txt` that lists the necessary packages (Flask in this case).  The `CMD` instruction is also corrected to use a more robust and common practice for running a web app in a Docker container. 

# REMINDER: as stated in the 'about' section, this is a deprecated repo, & I do not check it very often, nor do I actively maintain it.  Please feel free to fork, copy/paste, etc as you see fit.  You are welcome to submit PRs, but please do so with the knowledge that I might not see the PR for a very long time.

# node-red-contrib-send-multipart
This is a node-red node for posting http(s) requests containing files as multipart formData. Currently a work in progress.
As of now this node is only looking for files. However, there are future plans to handle all multipart/form-data.

## Installation
run npm -g install node-red-contrib-send-multipart

## Features
Pulled together using some of the best of parts of other node-red-contrib nodes (particularly node-red-contrib-http-request), and the best parts of stackoverflow.
Currently only sends files. However, there are future plans to handle other types multipart/form-data.

## Usage
Required inputs: url & filepath

Both can be indicated 2 ways:
1. Explicitly state the input on the node (e.g. filepath and/or url is a constant)
2. Pass the inputs into the node as part of the msg, as "msg.filepath" or "msg.url"


## Why this module?
As of May 2018, NodeRed does not yet support sending multipart form-data.  This module aims to begin to close that gap.

There is always room for improvement, and new ideas are valued.  Feel free to submit pull requests to make this library even better.

## What's next?
In the future, I definitely want to add more support for other data types, as well as more flexibility in the model.  For example, I'd for users to be able to just pass in a file instead of read it from local.  I developed this node for a very specific use case, which is why I haven't dived into all that yet.  It's on my to-do list!

# Installation instructions

```
curl -sLO git.io/kubectl-honk
chmod +x kubectl-honk
sudo mv kubectl-honk /usr/local/bin
```

# How to run

```
kubectl honk
```

# What is this?

If you ran `kubectl honk` and saw:

```
 _   _  ___  _   _ _   ___ _
| | | |/ _ \| \ | | | / / | |
| |_| | | | |  \| | |/ /| | |
|  _  | | | |     |   < |_|_|
| | | | |_| | |\  | |\ \ _ _
|_| |_|\___/|_| \_|_| \_(_|_)

Not the output you were expecting?
Relax, you have only been h0nX0r3d, not hacked.
For more information on why you are seeing this:
https://github.com/bgeesaman/kubectl-honk
```

and you followed that link here, you might be wondering how and why that happened.

First things first: __you have not been hacked, but you came very close__.  Your system either directly or indirectly ran this plugin, but I assure you, it's relatively benign and only prints out some sensitive pieces of information to stdout along with this warning message.

When using kubectl plugins, be sure to vet the source--you are essentially allowing plugin code to do whatever you would have permission to do on your local system, in your cluster, or even in your cloud account.  Stay safe out there.

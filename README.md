[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

# A hitchhiker's guide to a Google Cloud CTF

:warning: **This repository contains only the hints and instructions for the challenge.**:warning: 

:warning: **For the full Terraform setup and solutions - visit this [repository](https://github.com/n0jam/gcp-ctf-workshop)** :warning: 


## Your Goal

Your goal of this CTF is to exploit a vulnerable GCP project and find up to 5 flags.
During the challenge you will be able to move through the environment and step by step escalate your privileges until you manage the IAM bindings on the project, essentially allowing you to gain control of all resources in the project.
(In our CTF workshop setup, we have to keep you in check a bit and you will only be able to manage specific IAM bindings.)

## Prerequisites

To play this CTF and participate in our workshop you will need:
- A notebook and an internet connection
- A Google account. Any Google account such as `your-throwaway@gmail.com ` is enough. It does not have to be a Google Cloud account. 
- The [gcloud](https://cloud.google.com/sdk/docs/install) command line utility installed on your computer.

## Your starting point

The cloud services in the project might be misconfigured or leak information that can be useful for you as an attacker.
You'll start out with just an IP address as your first piece of information.

> [!NOTE]
> IP address to start with: `34.23.127.178`

We are providing you with useful hints and commands for each challenge.
Don't hesitate to use them, as you will have limited time for this CTF during our workshop.

## Challenges

- [Challenge 1](docs/challenge1.md)
- [Challenge 2](docs/challenge2.md)
- [Challenge 3](docs/challenge3.md)
- [Challenge 4](docs/challenge4.md)
- [Bonus Challenge 5](docs/challenge5.md)

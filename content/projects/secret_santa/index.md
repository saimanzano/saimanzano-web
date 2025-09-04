---
title: "Secret Santa"
date: 2025-09-04

tags: ["Projects","Data-viz","Phylogeny"]
author: "Saioa Manzano-Morales"
description: "This is the code for a Secret Santa generator." 
summary: "This is the code for a Secret Santa generator.." 
cover:
    image: "secret_santa.png"
    alt: "Secret Santa"
    relative: true
editPost:
    URL: "https://github.com/saimanzano/SecretSanta"
    Text: "GitHub repo"
showToc: true
disableAnchoredHeadings: false

---

Requires installing R libraries "argparse" and "blastula" which is handled automatically by the script via library "Pacman".

For the emails, you will require the "app password" from that gmail address. Please see how to obtain it from: https://rstudio.github.io/blastula/articles/sending_using_smtp.html

usage: 

```
SecretSanta.R [-h] [-e EMAIL] [-p PARTICIPANTS] [-a ADDITIONAL]

```

options:

-e EMAIL, --email EMAIL email address for the notifications to be sent from. Must be gmail
-p PARTICIPANTS, --participants PARTICIPANTS CSV file with following fields: name, email, ban(s). Bans are matches that cannot be made (e.g so that couples are not matched to each other). Can be more than one ban, separated by anything other than a comma.
-a ADDITIONAL, --additional ADDITIONAL Character string with additional info you want on the email (e.g budget, deadline, etc). Default: "Have fun!"
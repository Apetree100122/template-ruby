# Radio Frequency Key Fob Cloning

## Overview

<!--
Provide a 1-2 sentence description - see http://cveproject.github.io/docs/content/key-details-phrasing.pdf for tips

This format is a good guide:
[VULNTYPE] in [COMPONENT] in [APPLICATION] allows [ATTACKER] to [IMPACT] via [VECTOR] 
-->

The {{target}} and/or {{application}} allows a malicious attacker to clone a keyfob of any make/model

## Walkthrough & PoC

<!--
Provide a step-by-step walkthrough on how to access the vulnerable injection point, and how to exploit the vulnerability.
Adding a dot-pointed walkthrough with relevant screenshots will speed triage time and result in faster rewards!
-->

1. Setup {{hardware}} and {{software}} stack by {{action}}

1. Use the {{application}} on {{target}} to clone key fob by {{action}}

1. Use the original key fob to roll the nonce, then unlock {{target}} using spoofed {{hardware}} 


## Vulnerability Evidence

<!--
Your submission MUST include evidence of the vulnerability and not be theoretical in nature.

For an infotainment vulnerability, please include detailed instructions that can be followed to easily demonstrate and reproduce the issue. 
-->

The image(s) below demonstrates the cloning of a key fob to when the {{target}} is successfully unlocked or locked:

{{screenshot}}

## Demonstrated Impact

<!--
Attempt to completely stop the vehicle for functioning if the infotainment system controls mechanical aspect of the vehicle. If this is possible, provide a full proof-of-concept here.
--> 

A malicious attacker could exploit the {{target}} by creating a permanent clone of keys for {{target}} giving permanent access to any vehicle of the same make/model.


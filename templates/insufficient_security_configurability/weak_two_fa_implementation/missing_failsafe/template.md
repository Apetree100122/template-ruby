# 2FA Missing failsafe
## Overview
<!--
Provide a 1-2 sentence description - see http://cveproject.github.io/docs/content/key-details-phrasing.pdf for tips

This format is a good guide:
[VULNTYPE] in [COMPONENT] in [APPLICATION] allows [ATTACKER] to [IMPACT] via [VECTOR]


-->
Lack of a failsafe in the two factor authentication implementation in {{application}} of {{target}} allows a malicious attacker to {{action}}

## Walkthrough & PoC
<!--
Provide a step-by-step walkthrough on how to access the vulnerable injection point, and how to exploit the vulnerability.
Adding a dot-pointed walkthrough with relevant screenshots will speed triage time and result in faster rewards!

Example:

1. Login to in-scope asset at <www.inscope.com/login>
1. Browse to account page
1. Modify ID token to add single quote
1. View error which states 'SQL Syntax Error'
1. Replace ID value with `1' waitfor delay '00:00:10'; `
-->

1. Login to {{application}}
1. Navigate to the two factor authentication registration page at {{url}}
1. Register two factor authentication, and observe that the implementation provides no failsafe login methods, such as offline backup codes


## Vulnerability Evidence
<!--
Your submission MUST include evidence of the vulnerability and not be theoretical in nature.

For the lack of a failsafe in a two factor authentication implementation, please include a screenshot of the two factor authentication registration flow showing that no failsafe login method is provided.
-->

You can observe that {{application}} has no failsafe in the two factor authentication implementation below:

{{screenshot}}
## Demonstrated Impact
<!--
Envision how the lack of a failsafe in the two factor authentication implementation could be used in some impactful way. If a malicious action is possible, provide a full proof-of-concept here.
-->

Not providing a failsafe in the two factor authentication implementation in {{application}} could prevent a user who has lost their 2FA device to a malicious attacker from resetting the password of their account. This means that the malicious attacker could then perform {{action}}.
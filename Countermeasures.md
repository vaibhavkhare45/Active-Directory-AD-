🛡️ Active Directory Security Countermeasures
This document lists defensive strategies to mitigate common Active Directory (AD) attacks.
⚠️ These are best practices for securing enterprise environments.

1. 🏷️ Pass‑the‑Hash (PtH)
Defense:
   Enforce Privileged Access Workstations (PAWs).
   Use Windows Defender Credential Guard to protect NTLM hashes.
   Disable NTLM where possible; enforce Kerberos only.
   Monitor logins from unusual devices with SIEM.

2. 🎭 Pass‑the‑Ticket (PtT)
Defense:
   Regularly reset the KRBTGT account password (twice).
   Limit ticket lifetimes (TGT/TGS).
   Use LSASS protection to prevent credential dumping.
   Deploy Endpoint Detection and Response (EDR) tools

3. 🧩 Kerberoasting
Defense:
   Assign long, complex passwords for service accounts.
   Use Group Managed Service Accounts (gMSA).
   Limit service account privileges.
   Monitor Kerberos ticket requests for anomalies.

4. 👑 Golden Ticket Attack
Defense:
   Reset the KRBTGT password regularly.
   Monitor unusual authentication events (Event ID 4769, 4624).
   Restrict Domain Admin account use.
   Use a Tiered Admin model (no DA logins on workstations).

5. ⚔️ Silver Ticket Attack
Defense:
   Limit privileges of service accounts.
   Enable service account monitoring.
   Use Managed Service Accounts (MSAs).
   Detect suspicious TGS requests via SIEM.

6. 🌐 LDAP Enumeration
Defense:
   Limit anonymous LDAP binds.
   Restrict access to Active Directory Users & Computers (ADUC).
   Use LDAP signing and channel binding.
   Regularly audit AD permissions.

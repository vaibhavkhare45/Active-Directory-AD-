🔥 Common Active Directory Attacks
This document explains some of the most common attacks on Active Directory (AD) that penetration testers and attackers use.
⚠️ Note: These are for educational and lab purposes only.

1. 🏷️ Pass‑the‑Hash (PtH)
   Idea: Attackers use an NTLM hash of a password instead of the actual password to authenticate.
   Why Dangerous: No need to crack the hash — authentication works directly.
   Tools: Mimikatz, Impacket.

2. 🎭 Pass‑the‑Ticket (PtT)
   Idea: Attackers steal a Kerberos Ticket Granting Ticket (TGT) and reuse it to access resources.
   Why Dangerous: Provides domain‑wide access if high‑privilege tickets are stolen.
   Tools: Mimikatz, Rubeus.

3. 🧩 Kerberoasting
   Idea: Attackers request Kerberos service tickets and extract their hashes to brute‑force offline.
   Target: Service accounts with weak passwords.
   Tools: Rubeus, Impacket‑GetUserSPNs.

4. 👑 Golden Ticket Attack
   Idea: Attackers forge a Kerberos TGT using the KRBTGT account’s NTLM hash.
   Impact: Full domain compromise.
   Tools: Mimikatz.

5. ⚔️ Silver Ticket Attack
   Idea: Forging service tickets (TGS) for a specific service instead of the whole domain.
   Impact: Targeted persistence without touching domain controllers.
   Tools: Mimikatz.

6. 🌐 LDAP Enumeration
   Idea: Querying LDAP services to extract sensitive info like users, groups, and policies.
   Tools: ldapsearch, ADExplorer.
   

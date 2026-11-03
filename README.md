# Ahmed Pinger

Red teamer and offensive security engineer. I find out what somebody already
inside your network can reach, and then help make sure the next one gets caught.

CRTO, PNPT, Security+.

### What I'm doing now

**[Assumed Breach](https://www.assumed-breach.com)**, my offensive security
consultancy. Internal and
external [penetration tests](https://www.assumed-breach.com/services/penetration-testing),
[web](https://www.assumed-breach.com/services/web-application-testing) and
[API](https://www.assumed-breach.com/services/api-penetration-testing) work,
[AWS](https://www.assumed-breach.com/services/cloud-penetration-testing) and
[AI model](https://www.assumed-breach.com/services/ai-model-penetration-testing)
testing, [red team operations](https://www.assumed-breach.com/services/red-team-operations)
scoped by objective instead of by asset list, and
[incident response](https://www.assumed-breach.com/services/incident-response)
when something is already happening. Findings get ranked by what they let an
attacker do, not by raw CVSS, because a medium that chains into domain admin
matters more than a high nobody can reach. Every engagement ends with a retest,
because a report you cannot verify against is only half the work.

**i4 Ops**, where I am the attacker on a data exfiltration protection platform
so its defenses get measured instead of assumed. I write the exfiltration proofs
of concept in C, Go, Python and JavaScript, down to hand-built packets, and the
product has to stop all of them. I also run the security test cycles against the
product itself: RBAC and authorization test plans, end to end security test runs,
source code review, and the remediation tickets that come out of them.

### What I work on

**Networks and Active Directory.** Kerberoasting, RBCD, Shadow Credentials,
LAPS, AD CS templates, linked SQL servers, domain trusts: the walk from one weak
credential to domain admin. Cobalt Strike, Impacket, BloodHound, Burp.

**Cloud.** AWS. 20+ critical issues across five cloud environments,
including SSRF reached through a Lambda.

**Product and application security.** Web and API testing, source code review,
and the authorization work most scanners cannot do: RBAC matrices, role
boundaries, and multi-run regression testing to prove a fix held. Findings go out
as tickets an engineer can act on, not as a PDF.

**Endpoint and data exfiltration.** Building exfiltration primitives across
languages and down at the packet level, against products whose whole purpose is
to stop them. Linux internals, namespaces, syscall-level behavior.

**Detection engineering.** Graylog and Blumira, with around 100 TTPs mapped to
MITRE ATT&CK so rules match behavior instead of strings. I've written Windows
Defender bypasses whose techniques ended up in 10+ vendor products, which is the
part I'm actually pleased about: the bypass fed back into the detection.

**Infrastructure.** Terraform, Ansible, Docker. I build attack ranges as code,
which took exercise setup from days to hours, roughly 75% off, across 15+
corporate exercises. I also build the other side: fleet agents in Go, control
planes on Postgres and Redis, self-hosted deployments. It is easier to attack a
system when you have had to run one.

**AI.** The model serving and RAG pipelines now sitting inside products and
getting treated as if they were not attack surface. I have also done research on
detecting synthetic and deepfake media, building the forensic pipelines and NLP
models and scoring them on precision, recall, F1 and ROC-AUC.

### Security training

Teaching is a real part of the work, not a sideline.

- Around **120 professionals** trained hands-on in attack and defense technique.
- **12+ Active Directory focused CTF events** designed and run end to end, from
  the range build to the flags to the debrief.
- Security awareness training for teams that need the threat to feel real rather
  than theoretical.

### Things I've built

**[argument-injection-flags](https://github.com/AhmedPinger/argument-injection-flags)**
GTFOArgs tells you which flags are dangerous. I wanted to know which of them are
real on the host in front of me, so this one runs them. 45 entries, 21 with
executable probes, 12 primitives proven by execution on a stock macOS host. A
flag in a man page and a flag that actually spawns a process are different facts,
and only one of them helps you on an engagement.

**[RedTeamCTFs](https://github.com/AhmedPinger/RedTeamCTFs)**
Full walkthroughs of two Active Directory attack paths, command by command:
Jenkins credential passback, LAPS, ASREPRoasting, linked MSSQL abuse, DPAPI,
AD CS templates, trust abuse, and both flavours of constrained delegation.

**[Secure-Password-Storage](https://github.com/AhmedPinger/Secure-Password-Storage)**
Salted, iterated hashing and constant-time verification written from primitives
rather than by importing bcrypt, because that is the only way to see why each of
the three pieces exists.

### Writing

I write at [assumed-breach.com/blog](https://www.assumed-breach.com/blog). One
named vulnerability per post: what it actually is, how it gets exploited in
practice, and what to change so it stops working. The same posts are also on
[Medium](https://medium.com/@pingerahmed).

- [Pickle is a code format, not a data format](https://www.assumed-breach.com/blog/deserialization)
- [Argument injection and CVE-2024-4577 explained](https://www.assumed-breach.com/blog/argument-injection)
- [Server-side template injection](https://www.assumed-breach.com/blog/ssti)

### Contact

[assumed-breach.com](https://www.assumed-breach.com) ·
[LinkedIn](https://www.linkedin.com/in/ahmedpinger/) ·
[Medium](https://medium.com/@pingerahmed) ·
[Book a call](https://cal.com/ahmedp/discovery-call)

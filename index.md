Computer systems security notes (6.858, Fall 2014)
==================================================

Lecture notes from 6.858, taught by [Prof. Nickolai Zeldovich](http://people.csail.mit.edu/nickolai/) and [Prof. James Mickens](http://research.microsoft.com/en-us/people/mickens/) in 2014. These lecture notes are slightly modified from the ones posted on the 6.858 [course website](http://css.csail.mit.edu/6.858/2014/schedule.html).

 * Lecture **1**: [Introduction](l01-intro.html): what is security, what's the point, no perfect security, policy, threat models, assumptions, mechanism, buffer overflows
 * Lecture **2**: [Control hijacking attacks](l02-baggy.html): buffer overflows, stack canaries, bounds checking, electric fences, fat pointers, shadow data structure, Jones & Kelly, baggy bounds checking
 * Lecture **3**: [More baggy bounds and return oriented programming](l03-brop.html): costs of bounds checking, non-executable memory, address-space layout randomization (ASLR), return-oriented programming (ROP), stack reading, blind ROP, gadgets
 * Lecture **4**: [OKWS](l04-okws.html): privilege separation, Linux discretionary access control (DAC), UIDs, GIDs, setuid/setgid, file descriptors, processes, the Apache webserver, chroot jails, remote procedure calls (RPC)
 * Lecture **5**: **Penetration testing** _guest lecture_ by Paul Youn, iSEC Partners
 * Lecture **6**: [Capsicum](l06-capsicum.html): confused deputy problem, ambient authority, capabilities, sandboxing, discretionary access control (DAC), mandatory access control (MAC), Capsicum
 * Lecture **7**: [Native Client (NaCl)](l07-nacl.html): sandboxing x86 native code, software fault isolation, reliable disassembly, x86 segmentation
 * Lecture **8**: [Web Security, Part I](l08-web-security.html): modern web browsers, same-origin policy, frames, DOM nodes, cookies, cross-site request forgery (CSRF) attacks, DNS rebinding attacks, browser plugins
 * Lecture **9**: [Web Security, Part II](l09-web-defenses.html): cross-site scripting (XSS) attacks, XSS defenses, SQL injection atacks, Django, session management, cookies, HTML5 local storage, HTTP protocol ambiguities, covert channels
 * Lecture **10**: **Symbolic execution** _guest lecture_ by Prof. Armando Solar-Lezama, MIT CSAIL
 * Lecture **11**: **Ur/Web** _guest lecture_ by Prof. Adam Chlipala, MIT, CSAIL
 * Lecture **12**: [TCP/IP security](l12-tcpip.html): threat model, sequence numbers and attacks, connection hijacking attacks, SYN flooding, bandwidth amplification attacks, routing
 * Lecture **13**: [Kerberos](l13-kerberos.html): Kerberos architecture and trust model, tickets, authenticators, ticket granting servers, password-changing, replication, network attacks, forward secrecy
 * Lecture **14**: [ForceHTTPS](l14-forcehttps.html): certificates, HTTPS, Online Certificate Status Protocol (OCSP), ForceHTTPS
 * Lecture **15**: **Medical software** _guest lecture_ by Prof. Kevin Fu, U. Michigan
 * Lecture **16**: [Timing attacks](l16-timing-attacks.html): side-channel attacks, RSA encryption, RSA implementation, modular exponentiation, Chinese remainder theorem (CRT), repeated squaring, Montgomery representation, Karatsuba multiplication, RSA blinding, other timing attacks
 * Lecture **17**: [User authentication](l17-authentication.html): what you have, what you know, what you are, passwords, challenge-response, usability, deployability, security, biometrics, multi-factor authentication (MFA), MasterCard's CAP reader
 * Lecture **18**: [Private browsing](l18-priv-browsing.html): private browsing mode, local and web attackers, VM-level privacy, OS-level privacy,  OS-level privacy, what browsers implement, browser extensions 
 * Lecture **19**: **Tor** _guest lecture_ by Nick Mathewson, Tor Project
   + 6.858 notes from 2012 on [Anonymous communication](l19-tor.html): onion routing, Tor design, Tor circuits, Tor streams, Tor hidden services, blocking Tor, dining cryptographers networks (DC-nets)
 * Lecture **20**: [Mobile phone security](l20-android.html): Android applications, activities, services, content providers, broadcast receivers, intents, permissions, labels, reference monitor, broadcast intents
 * Lecture **21**: [Information flow tracking](l21-taintdroid.html): TaintDroid, Android data leaks, information flow control, taint tracking, taint flags, implicit flows, x86 taint tracking, TightLip
 * Lecture **22**: **MIT's IS&T** _guest lecture_ by Mark Silis and David LaPorte, MIT IS&T
 * Lecture **23**: [Security economics](l23-click-trajectories.html): economics of cyber-attacks, the spam value chain, advertising, click-support, realization, CAPTCHAs, botnets, payment protocols, ethics

### New notes from 2015

 * Lecture **8**: [Intel Software Guard Extensions (SGX)](2015/l08-sgx.html): isolation, Iago attacks, enclaves, attestation, Haven

Papers
------

List of papers we read ([papers/](papers/)):

 - [Baggy bounds checking](papers/baggy.pdf)
 - [Hacking blind](papers/brop.pdf)
 - [OKWS](papers/okws.pdf)
 - [The confused deputy](papers/confused-deputy.pdf) (or why capabilities might have been invented)
 - [Capsicum](papers/capsicum.pdf) (capabilities)
 - [Native Client](papers/nacl.pdf) (sandboxing x86 code)
 - [OWASP Top 10](papers/owasp-top-10.pdf), the most critical web application security risks
 - [KLEE](papers/klee.pdf) (symbolic execution)
 - [Ur/Web](papers/urweb.pdf) (functional programming for the web)
 - [A look back at "Security problems in the TCP/IP protocol suite"](papers/lookback-tcpip.pdf)
 - [Kerberos](papers/kerberos.pdf): An authentication service for open network systems
 - [ForceHTTPs](papers/forcehttps.pdf)
 - [Trustworthy Medical Device Software](papers/medical-sw.pdf)
 - [Remote timing attacks are practical](papers/brumley-timing.pdf)
 - [The quest to replace passwords](papers/passwords.pdf)
 - [Private browsing modes](papers/private-browsing.pdf)
 - [Tor](papers/tor-design.pdf): the second-generation onion router
 - [Understanding Android security](papers/android.pdf)
 - [TaintDroid](papers/taintdroid.pdf): an information-flow tracking system for realtime privacy monitoring on smartphones
 - [Click trajectories](papers/trajectories.pdf): End-to-end analysis of the spam value chain

### "Newer" papers

 - [Iago Attacks: Why the System Call API is a Bad Untrusted RPC Interface](https://cseweb.ucsd.edu/~hovav/dist/iago.pdf)

Other papers
------------

 - [The Chinese Wall Security Policy](papers/chinese-wall-sec-pol.pdf)

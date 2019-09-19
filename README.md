# Mixnet and ACN research

This is a collection of research on Mixnets and Anonymous Communication Networks (ACN) that is a part of a wider effort of research for a default transaction building method for [Grin](https://grin-tech.org). The list is non-exhaustive, focuses on recent advances that are relevant in the context of Grin, and doesn't include more classical work.

🔥: Recommended in particular in our context

### Library resources

* [Freehaven Anonymity Bibliography](https://www.freehaven.net/anonbib/full/topic.html)
* [Katzenpost Mixnet Academy](https://github.com/katzenpost/docs/blob/master/mixnet_academy/syllabus.rst)


### Table of contents

- [Mixnet and ACN research](#mixnet-and-acn-research)
    - [Library resources](#library-resources)
    - [Table of contents](#table-of-contents)
  - [Meta](#meta)
  - [Mixnets](#mixnets)
    - [General](#general)
    - [Protocols](#protocols)
    - [Packet formats](#packet-formats)
    - [Attacks](#attacks)
  - [Bulletin boards](#bulletin-boards)
  - [PIR](#pir)
  - [DHTs](#dhts)
  - [Contributing](#contributing)


## Meta

|Title|Author(s)|Year|Related info|
|:---|:---|---|:---|
[Why I'm not an entropist](https://www.freehaven.net/anonbib/cache/entropist.pdf) | Syverson | 2009 | |
[A terminology for talking about privacy by data minimization: Anonymity, Unlinkability, Undetectability, Unobservability, Pseudonymity, and Identity Management v0.34](http://dud.inf.tu-dresden.de/literatur/Anon_Terminology_v0.34.pdf) | Pfitzmann & Hansen | 2010 | |

## Mixnets

### General

|Title|Author(s)|Year|Related info|
|:---|:---|---|:---|
🔥 [Anonymity Trilemma: Strong Anonymity, Low Bandwidth Overhead, Low Latency—Choose Two](https://eprint.iacr.org/2017/954.pdf)| Das, Meiser, Mohammadi, Kate| 2018 | |
[Systematizing Decentralization and Privacy: Lessons from 15 Years of Research and Deployments](https://www.petsymposium.org/2017/papers/issue4/paper87-2017-4-source.pdf) | Troncoso, Isaakidis, Danezis, Halpin | 2017 | |
| [Impact of Network Topology on Anonymity and Overhead in Low-Latency Anonymity Networks](https://www.esat.kuleuven.be/cosic/publications/article-1230.pdf) | Diaz, Murdoch, Troncoso | 2010 | |
| [A Survey of Anonymous Communication Channels](https://www.esat.kuleuven.be/cosic/publications/article-927.pdf) | Danezis & Diaz | 2008 | |
| [On Privacy Notions in Anonymous Communication](http://orbilu.uni.lu/bitstream/10993/40073/1/1812.05638.pdf) | Kuhn, Beck, Schiffner, Jorswieck, Strufe | 2019 | |
[A Survey on Measuring Anonymity in Anonymous Communication Systems](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8723335) | Lu, Du, Wang | 2019 | |

### Protocols

|Title|Author(s)|Year|Related info|
|:---|:---|---|:---|
[A Universally Composable Framework for the Privacy of Email Ecosystems](https://eprint.iacr.org/2018/848.pdf) | Chaidos, Fourtounelli, Kiayias, Zacharias | 2018 | |
| [MCMix: Anonymous Messaging via Secure Multiparty Computation](https://eprint.iacr.org/2017/778.pdf) | Alexopoulos, Kiayias, Talviste, Zacharias | 2017 | |
[HORNET: High-speed Onion Routing at the Network Layer](https://www.scion-architecture.net/pdf/2015-HORNET.pdf) | Chen, Asoni, Barrera, Danezis, Perrig | 2015 | |
[Atom: Horizontally Scaling Strong Anonymity](https://people.csail.mit.edu/henrycg/files/academic/papers/sosp17atom.pdf) |Kwon, Corrigan-Gibbs, Devadas,  Ford | 2017 | |
[Fully Non-Interactive Onion Routing with Forward- Secrecy](http://www.dmi.unict.it/diraimondo/web/wp-content/uploads/papers/fsor-journal.pdf) | Catalano, Di Raimondo, Fiore, Gennaro, Puglisi | 2013 | |
|[Two Cents for Strong Anonymity: The Anonymous Post-office Protocol](https://eprint.iacr.org/2016/489.pdf) | Gelernter, Herzberg, Leibowitz | 2016 | |
|[TARANET: Traffic-Analysis Resistant Anonymity at the Network Layer](https://netsec.ethz.ch/publications/papers/chen_taranet_eurosp18.pdf)| Chen, Barrera, Asoni, Danezis, Perrig, Troncoso | 2018 | |
| [Provably Secure and Practical Onion Routing](https://www.cosic.esat.kuleuven.be/ecrypt/provpriv2012/abstracts/backes.pdf) |Backes, Goldberg, Kate,  Mohammadi | 2012 | |
| [TASP: Towards Anonymity Sets that Persist](https://www.freehaven.net/anonbib/cache/tasp-wpes16.pdf) | Hayes, Troncoso, Danezis | 2016 | |
| 🔥 [The Loopix Anonymity System](https://arxiv.org/abs/1703.00536) | Piotrowska, Hayes, Elahi, Meiser, Danezis | 2017 | <ul><li>[Video & Slides](https://www.usenix.org/conference/usenixsecurity17/technical-sessions/presentation/piotrowska)</li><li>[Python reference implementation](https://github.com/UCL-InfoSec/loopix)</li></ul> | 
| 🔥 [Vuvuzela: Scalable Private Messaging Resistant to Traffic Analysis](https://pdos.csail.mit.edu/papers/vuvuzela:sosp15.pdf) | van den Hooff, Lazar, Zaharia, Zeldovich | 2015 | <ul><li>[Website](https://vuvuzela.io)</li><li>[Go Implementation](https://github.com/vuvuzela/vuvuzela)</li></ul>
[HoneyBadgerMPC and AsynchroMix: Practical Asynchronous MPC and its Application to Anonymous Communication](https://eprint.iacr.org/2019/883.pdf) |Lu, Yurek, Kulshreshtha, Govind, Mahadev, Kate, Miller | 2019 | |
[Stadium: A Distributed Metadata-Private Messaging System](https://eprint.iacr.org/2016/943.pdf) | Tyagi, Gilad, Leung, Zaharia, Zeldovich | 2016 | |
[Karaoke: Distributed Private Messaging Immune to Passive Traffic Analysis](https://www.usenix.org/system/files/osdi18-lazar.pdf) | Lazar, Gilad, Zeldovich | 2018 | <ul><li>[Slides & Audio](https://www.usenix.org/conference/osdi18/presentation/lazar)</li></ul> |


### Packet formats

|Title|Author(s)|Year|Related info|
|:---|:---|---|:---|
 🔥[Sphinx: A Compact and Provably Secure Mix Format](https://cypherpunks.ca/~iang/pubs/Sphinx_Oakland09.pdf) | Danezis & Goldberg | 2009 | <ul><li>[Specification](https://github.com/katzenpost/docs/blob/master/specs/sphinx.rst)</li><li>[Rust implementation](https://github.com/sphinx-cryptography/rust-sphinxcrypto)</li></ul> |
[Using Sphinx to Improve Onion Routing Circuit Construction (short paper)](https://www.freehaven.net/anonbib/cache/sphinx-onion-fc10.pdf) | Kate & Goldberg | 2010 | |
 
 ### Routing

|Title|Author(s)|Year|Related info|
|:---|:---|---|:---|
| 🔥 [Multiparty Routing: Secure Routing for Mixnets](https://arxiv.org/pdf/1708.03387.pdf) | Shirazi, Andreeva, Kohlweiss, Diaz | 2017 | |
| 🔥 [A Survey on Routing in Anonymous Communication Protocols](https://publications.cispa.saarland/2613/2/a51-shirazi.pdf) | Shirazi, Simeonowski, Asghar, Backes, Diaz | 2018 | |
| 🔥 [Alpenhorn: Bootstrapping Secure Communication Without Leaking Metadata]() | Lazar & Zeldovich | 2016 | <ul><li>[Website](https://vuvuzela.io)</li><li>[Go Implementation](https://github.com/vuvuzela/alpenhorn)</li></ul> |

### Attacks

|Title|Author(s)|Year|Related info|
|:---|:---|---|:---|
| 🔥 [Limits of Anonymity in Open Environments](https://www.freehaven.net/anonbib/cache/limits-open.pdf)  | Kedogan, Agrawal, Penz | 2002 | |
🔥[An Empirical Study of the I2P Anonymity Network and its Censorship Resistance](https://www3.cs.stonybrook.edu/~mikepo/papers/i2p.imc18.pdf) | Hoang, Antonakakis, Kintis, Polychronakis | 2018 |  |
🔥[Anonymity Services Tor, I2P, JonDonym: Classifying in the Dark (Web)](https://domenicociuonzo.files.wordpress.com/2018/02/ieee_tdsc.pdf) |  Montieri, Ciuonzo, Aceto, Pescapé | 2018 ||
[Sleeping dogs lie on a bed of onions but wake when mixed](https://petsymposium.org/2011/papers/hotpets11-final10Syverson.pdf) | Syverson | 2011 | |
|[Using Linkability Information to Attack Mix-Based Anonymity Services](https://www.esat.kuleuven.be/cosic/publications/article-1215.pdf) | Schiffner & Clauß | 2009 | |
| [Statistical Disclosure Attacks on Anonymity Systems](http://www0.cs.ucl.ac.uk/staff/G.Danezis/papers/PoolSDA3.pdf) | Danezis & Serjantov | 2004 | |
| [Statistical Disclosure Attacks: Traffic Confirmation in Open Environments](http://www0.cs.ucl.ac.uk/staff/G.Danezis/papers/StatDisclosure.pdf) | Danezis | 2003 | |
| [Analysis of Fingerprinting Techniques for Tor Hidden Services](https://www.freehaven.net/anonbib/cache/fingerprinting-wpes17.pdf) | Panchenko, Mitseva, Henze, Lanze, Wehrle, Engel  | 2017 | |
| [Traffic Analysis Attacks and Trade-Offs in Anonymity Providing Systems](http://www.cypherspace.org/adam/pubs/traffic.pdf) |  Back, Möller, Stiglic |  2001 | |
[No Right to Remain Silent: Isolating Malicious Mixes](https://www.usenix.org/system/files/sec19-leibowitz.pdf) | Leibowitz, Piotrowska, Danezis, Herzberg| 2019 | |

## Bulletin boards

|Title|Author(s)|Year|Related info|
|:---|:---|---|:---|
[Privately (and Unlinkably) Exchanging Messages Using a Public Bulletin Board](https://www.cs.ru.nl/~jhh/publications/abb-wpes.pdf) | Hoepman | 2015 | |
[A Private and Unlinkable Message Exchange Using a Public bulletin board in Opportunistic Networks](https://arxiv.org/abs/1909.02380) | Farkhondeh | 2019 | |
[Simple and Efficient Approach for Achieving End-to-End Anonymous Communication](https://eprint.iacr.org/2019/790.pdf) | Jiang, Bowers, Lin | 2019 | |

## PIR

|Title|Author(s)|Year|Related info|
|:---|:---|---|:---|
[The Pynchon Gate](https://www.freehaven.net/anonbib/cache/sassaman:wpes2005.pdf) | Sassaman, Cohen, Mathewson | 2005 | |

## DHTs

|Title|Author(s)|Year|Related info|
|:---|:---|---|:---|
[Fundamental Design Issues in Anonymous Peer-to-peer Distributed Hash Table Protocols](https://www.researchgate.net/profile/Todd_Baumeister/publication/334729155_Fundamental_Design_Issues_in_Anonymous_Peer-to-peer_Distributed_Hash_Table_Protocols/links/5d3cfdf1a6fdcc370a660bcd/Fundamental-Design-Issues-in-Anonymous-Peer-to-peer-Distributed-Hash-Table-Protocols.pdf) | Baumeister | 2019 | |

## Contributing
Pull requests are welcomed! Help propose research to add to the list and help with the grouping and analysis. 💟

---
title: QUIC Protocol
date: 2020-03-12T18:07:16.000+06:00
thumbnail: images/portfolio/QUIC.jpeg
service: Java, Socket Programming, Junit Test
client: Adv Data Communication, CSI 5321, Baylor University
shortDescription: QUIC (Quick UDP Internet Connections) is a new transport protocol for the internet, developed by Google.

  QUIC solves a number of transport-layer and application-layer problems experienced by modern web applications, while requiring little or no change from application writers. QUIC is very similar to TCP+TLS+HTTP/2, but implemented on top of UDP. Having QUIC as a self-contained userspace protocol allows innovations which aren’t possible with existing protocols as they are hampered by legacy clients and middleboxes. 
challenge: Main challenge was to manage congestion control over UDP protocol. UDP is not designed for this kind of task.
solution: To manage congestion control we have follow the strategy which is described in google official website. It is a mechnism of attaching some extra information with actual data.

---

---
permalink: /index.html
---


# Cheops for the Edge

## What is Cheops?

Cheops is a service mesh used to geo-distribute Cloud Applications for
Edge computing.



### Move your applications from the Cloud to the Edge


The Edge paradigm allows the applications to be executed closer to the
user.  Latency and privacy concerns are important reasons to motivate
the use of Edge infrastructures for applications.  But deploying an
application to the Edge is different from deploying the same
application in a few, well controlled datacenters.


<img width="400" align='right' src="/assets/img/edge-infra.png">
<p><em>The Cloud and Edge infrastructure considered here.</em></p>


Edge infrastructures imply less resources on each location, increased
latency for requests between locations, and more disconnections and
failures.  However, Cloud applications were not developped with these
constraints in mind, and worse, are probably expecting the requests
between services to be made on the same location.


To allow the use of Cloud applications to the Edge without changing
their code, a solution to geo-distribute them is required.

**Cheops is such a solution.**

It relies on a fully distributed approach, where the application it
geo-distributes is deployed on every sites of the infrastructure,
along with Cheops.  This way, each instance of the application can run
in isolation as it is fully deployed.

But to leverage the entire infrastructure, Cheops allows
collaborations between those instances. Three types of collaborations
were envisioned to help the users fulfill their needs.

To use these collaborations, a DSL called scope-lang was created to
allow users to specify where and how (the scope) they want their
application resources to be distributed, for each resource.  It is
used naturally, using the native command from the application enriched
with the scope and sending it to Cheops.

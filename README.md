# Cross-Layer Optical I/O Architecture for Heterogeneous Accelerators

## Status

**Research project in development. Architecture accepted and owner-frozen; experimental results are not yet claimed.**

No simulation, measurement, benchmark, verification or validation result should be inferred from the repository structure alone.

## Research problem

Accelerator I/O must trade bandwidth, reach, power, latency, reliability and physical density. Electrical channels incur channel-loss and SerDes costs; optical links introduce laser/source, modulation, coupling, receive and thermal/static costs. This project asks which architecture is favourable under a common post-PHY service boundary and complete boundary accounting rather than assuming that optical I/O is intrinsically superior.

## Frozen comparison

The primary study compares:

- a real electrical link;
- fewer/faster optical lanes; and
- more/slower spectral-WDM optical lanes.

The owner-frozen Core uses O-band direct-detection ring-WDM, an 800-Gb/s one-way post-PHY primary service demand, a 1024-Gb/s realistic-bundle quantisation sensitivity, a 1-m common-endpoint primary comparison, 10/100-m optical reach sensitivities, N={8,16,32}, and a 3.2-THz allocated spectral budget.

## Methodology

Planned evidence paths include:

- public Touchstone channel data and mixed-mode S-parameter analysis;
- official COM methodology and electrical-link/SerDes abstraction;
- first-party MODE/FDE and EME optical anchors;
- INTERCONNECT-level link modelling;
- complete source-to-destination energy and latency accounting;
- utilisation, temperature, reach and reliability sensitivities;
- coherent technology bundles and uncertainty/regime maps; and
- a service-envelope export for Projects 03 and 04.

## Evidence discipline

Imported measurements remain attributed to their original platforms. Modelled or simulated quantities are not presented as measurements. No proprietary NVIDIA or OLIX architecture is claimed. Empty directories indicate planned work only.

## Portfolio interface

P02 exports physical/link-service quantities such as post-PHY capacity, physical/PHY latency, physical power terms, mapping, skew, reliability/error abstraction, uncertainty and validity. P03 owns digital framing/deskew/flow-control behaviour. P04 owns workload serialization, dynamic queueing, congestion and system consequences.

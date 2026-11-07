# Energy Consumption of the DTSVLIW Architecture (WSCAD 2004)

**Original title:** *O Consumo de Energia da Arquitetura DTSVLIW*  
**Authors:** Felipe Thomaz Pedroni, Fernando Líbio L. Almeida, and Alberto F. De Souza  
**Affiliation:** Universidade Federal do Espírito Santo (UFES), Brazil  
**Conference:** 5th Workshop de Computação de Alto Desempenho (WSCAD 2004), Foz do Iguaçu, Brazil, October 27–29, 2004  
**Published paper:** [https://doi.org/10.5753/wscad.2004.19004](https://doi.org/10.5753/wscad.2004.19004)

## About this work

This paper investigates the estimated dynamic and static power consumption of the **Dynamically Trace Scheduled Very Long Instruction Word (DTSVLIW)** processor architecture and compares it with an Alpha 21264-based superscalar processor model.

We extended a DTSVLIW simulator written in C and running on Linux to incorporate architectural power models derived from **Wattch** and **Hotleakage**. The evaluation used **SPEC CPU2000** workloads and simulator configurations based on the **SimpleScalar 3.0** framework. Experiments were run using the UFES/LCAD research computing cluster.

The DTSVLIW architecture combines a scalar execution mode, which dynamically constructs VLIW instruction blocks, with a VLIW execution mode that reuses those blocks. The study examines how this organization affects modeled power dissipation relative to the superscalar reference architecture.

## Reported results

For the evaluated **180 nm** configuration, the paper reports the following average reductions in **modeled power dissipation** relative to the Alpha 21264 reference:

| Workload category         | DTSVLIW | Alpha 21264 | Reported reduction |
| ------------------------- | ------: | ----------: | -----------------: |
| Integer benchmarks        | 14.80 W |     23.54 W |         **37.12%** |
| Floating-point benchmarks | 13.06 W |     17.63 W |         **25.92%** |

These are **simulation-based estimates**, not power measurements from manufactured DTSVLIW silicon. The results depend on the processor models, workloads, and technology assumptions used in the 2004 study. The paper also discusses static power trends across process technologies.

## Papers

- [**Original conference paper (Portuguese)**](papers/Pedroni_2004_WSCAD_Original_PT.pdf)
- [**English translation**](papers/Pedroni_2004_WSCAD_English_Translation.pdf)
- [**Official publication (DOI)**](https://doi.org/10.5753/wscad.2004.19004)

> **Translation note:** The English version is an AI-assisted translation of the paper originally published in Portuguese in 2004. It is provided to make the work easier to read internationally; it is **not** a separate peer-reviewed publication. In case of any discrepancy, the original published paper is authoritative. Some labels embedded in the original figures may remain in Portuguese.

## Presentation

This work was presented at **WSCAD 2004** in Foz do Iguaçu, Brazil. The paper is the available public record of the research and its experimental methodology; this repository does not claim to contain the original presentation slides or a recording.

## Citation

Pedroni, F. T., Almeida, F. L. L., and De Souza, A. F. (2004). *O Consumo de Energia da Arquitetura DTSVLIW*. Workshop de Computação de Alto Desempenho (WSCAD 2004). https://doi.org/10.5753/wscad.2004.19004

## Publication and reuse

The DOI points to the published proceedings. Availability of a PDF in this repository should not be interpreted as an additional license or permission to republish third-party material. Refer to the original publisher for applicable reuse terms.

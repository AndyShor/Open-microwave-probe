# Low cost high frequency 1-20 GHz near field probes.

![](\Open_probe.jpg)

These near field probes are an adaptation of design proposed in [1-3] for a magnetic loop and an electric  probes for wide frequency range of 1-20 GHz and high spatial resolution, thanks to small size of the sensing part.
In [1] authors propose to make the probe using FR4 laminate for cost reasons despite FR4 poor performance at higher frequencies. This particular realization is also an amateur tool and not meant to be especially precise and reproducible from one manufactured probe to another. But it allows to have some understanding of high frequency EMC with good spatial resolution and probes costing under 100$ for a small batch.
Probes were designed in KiCAD and manufactured using JLCPCB. Due to limited available options the stack-up and the thickness are not exactly the same as assumed in the original design, other features such as small vias could be in general produced. For edge mounted SMA connector I used Amphenol 901-10511-2 SMA connectors because of small central pin, that is easier to couple to coplanar waveguide input. Similar connectors can be seen in the original publication [1]. Soldering is a bit tricky and was performed using a hot air gun.
For further readings on the topic of near-field high frequency probes I can recommend a few other articles. General theory of loop antenna as a probe [4,5]. Equivalent scheme analysis of a loop probe [6].  With higher budget and access to more customized PCB manufacturing much more high-end probes could be produced following the ideas and examples laid out in the literature [7-9]. If you don’t have institutional access to paywalled publication read this first https://en.wikipedia.org/wiki/Sci-Hub, some of the listed publications such as [6] are Open Access.
If you feel fancy and have access to thin film technology instead of PCB there are some proposed designes as well [10,11].

This repo contains gerber files sufficient for manufacturing as well as original KiCAD files. For KiCAD files you will need to add mouse bite footprint used to join electric and magnetic probes into 1 PCB.

[1] Namahoot A, Akkaraekthalin P, Chalermwisutkul S. Design of a low-cost 1-20 GHz magnetic near-field probe with FR-4 printed circuit board. Int J RF Microw Comput Aided Eng. 2019; 29:e21958. https://doi.org/10.1002/mmce.21958

[2] Z. Yan, J. Wang, W. Zhang, Y. Wang and J. Fan, "A Miniature Ultrawideband Electric Field Probe Based on Coax-Thru-Hole via Array for Near-Field Measurement," in IEEE Transactions on Instrumentation and Measurement, vol. 66, no. 10, pp. 2762-2770, Oct. 2017, doi: 10.1109/TIM.2017.2681282.

[3] Z. Yan, J. Wang, W. Zhang, Y. Wang and J. Fan, "A Simple Miniature Ultrawideband Magnetic Field Probe Design for Magnetic Near-Field Measurements," in IEEE Transactions on Antennas and Propagation, vol. 64, no. 12, pp. 5459-5465, Dec. 2016, doi: 10.1109/TAP.2016.2606556.

[4] H. Whiteside and R. King, "The loop antenna as a probe," in IEEE Transactions on Antennas and Propagation, vol. 12, no. 3, pp. 291-297, May 1964, doi: 10.1109/TAP.1964.1138213.

[5] J. Dyson, "Measurement of near fields of antennas and scatterers," in IEEE Transactions on Antennas and Propagation, vol. 21, no. 4, pp. 446-460, July 1973, doi: 10.1109/TAP.1973.1140518.

[6] H. Funato and T. Suga, "Magnetic near-field probe for GHz band and spatial resolution improvement technique," 2006 17th International Zurich Symposium on Electromagnetic Compatibility, Singapore, 2006, pp. 284-287, doi: 10.1109/EMCZUR.2006.214926.

[7] J. Wang, Z. Yan, W. Liu, X. Yan and J. Fan, "Improved-Sensitivity Resonant Electric-Field Probes Based on Planar Spiral Stripline and Rectangular Plate Structure," in IEEE Transactions on Instrumentation and Measurement, vol. 68, no. 3, pp. 882-894, March 2019, doi: 10.1109/TIM.2018.2857898.

[8] Liu, J., Xiao, M., He, X., Fang, W., Shao, W., Huang, Q., Lu, G., Wang, L., Huang, Y., En, Y. and Yao, R. (2021), Symmetrical double-loop H-field probe with floating shield for improving sensitivity and electric field suppression. IET Microw. Antennas Propag, 15: 464-473. https://doi.org/10.1049/mia2.12050

[9] Y. -T. Chou and H. -C. Lu, "Magnetic Near-Field Probes With High-Pass and Notch Filters for Electric Field Suppression," in IEEE Transactions on Microwave Theory and Techniques, vol. 61, no. 6, pp. 2460-2470, June 2013, doi: 10.1109/TMTT.2013.2258034.

[10] Naoya Tamaki et al.  "A miniature thin-film shielded-loop probe with a flip-chip bonding for magnetic near field measurements", Electronics and Communications in Japan, Part 2, Vol. 88, No. 4, 2005, doi: 10.1002/ecjb.20091

[11] N. Ando et al., "Miniaturized thin-film magnetic field probe with high spatial resolution for LSI chip measurement," 2004 International Symposium on Electromagnetic Compatibility (IEEE Cat. No.04CH37559), Silicon Valley, CA, USA, 2004, pp. 357-362 vol.2, doi: 10.1109/ISEMC.2004.1349815.

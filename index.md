# [Precomputed Atmospheric Scattering](https://github.com/ebruneton/precomputed_atmospheric_scattering) for Thick Atmospheres

Original

![0](data/0.png)

Improve the scattering integration ([commit link](https://github.com/c52e/UnrealEngineSkyAtmosphere/commit/319d4c475b88b5635ccde315b0f1bd5054fa41b5))

![1](data/1.png)

Store optical length instead of transmittance to fix artifacts near the horizon ([commit link](https://github.com/c52e/UnrealEngineSkyAtmosphere/commit/e041eaa02086f34059015723376cee2771f6ba86))

![2](data/2.png)

Increase sample count ([commit link](https://github.com/c52e/UnrealEngineSkyAtmosphere/commit/a9971e90091e12098c03e997291852e864c0ff72))

![3](data/3.png)

[Multiple scattering LUT](https://sebh.github.io/publications/egsr2020.pdf) can be used to reduce the cost of precomputation.

Single scattering

![scattering1](data/scattering1.png)

9 order multiple scattering

![scattering9](data/scattering9.png)

Use multiple scattering LUT

![multiscatteringlut](data/multiscatteringlut.png)

With multiple scattering LUT, physically based overcast sky can be simulated by adding an additional dense mie scattering layer at altitudes of clouds.

With additional dense mie scattering layer

![overcast](data/overcast.png)

Without additional dense mie scattering layer

![clear](data/clear.png)

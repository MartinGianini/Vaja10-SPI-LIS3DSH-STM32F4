2.)

b)MISO: master input, slave output
MOSI - master sporoča, slave posluša 
SCK - urin takt, ki ga oddaja master 
SS - master določi, s katero slave komunicira (signal aktiven v nizkem stanju)

c)Enoti master.

e)PA6, PA7, PA8

g)PE3

h)16 (1,5 Mb/s je najbližje, kar lahko dosežem za 1 Mb/s)





Predlog za izboljšavo navodil:

2.)
Nastavitve za NVIC in GPIO se nahajajo v System View nad sliko pinout-a, poleg Pinout View

3.) 
d) in e) bi lahko bili spojeni v en del, saj e) prikazuje kodo v celoti;
v kodi pri e) je tiskarski škrat, HAL_SPI_Recieve bi moral biti HAL_SPI_Receive (poglejte "i" in "e")



//Sledil sem danim navodilom, kolikor so bili točni, a v STM Studi-u je Read value vedno 0, tudi s premikom
ploščice in resetiranjem (kot videno v demonstraciji). Težava je najverjetneje v sestavi kode same, če ni,
je potem težava z giroskopi obeh ploščic 32F4, ki sta navoljo.

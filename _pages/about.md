---
permalink: /about/
title: "About"
modified: 2020-07-25
---

{% include base_path %}
{% include toc %}

## About the IO/VCC

The IO/VCC was created in Jul 2020 by Carlos Delphino, Marcelo Samsoniuk and
Paulo Mathias after the analysis of a very weird segment of Verilog code:

```case(1'b1)
  RST: Q <= 1'b1;
  SET: Q <= 1'b0;
  default: Q <= D;
endcase```

After a short simulation with iverilog, we found that the code works and,
as expected, describes a flip-flop. After a brief discussion about the
better way to write the same thing, we found that there are lots of ways to
write it, in a way that the above way was really very obfuscated.

The discussion resulted in a joke about create a contest for obfuscated
verilog code, just like the well known contest for obfuscated C code
(IOCCC.org). As addition, Paulo observed that IO VCC is a well known term in
the FPGA area, which describes the voltage used in the IO pin.

Few seconds later Marcelo produced a draft of the IO/VCC logo, with the well
known tri-state IO buffer used in mostly FPGAs with an pull-up attached to
the IO signal. At same time, Carlos proposed create the site and here we
are! 

### About the IO/VCC Founders

*Carlos Delphino*

github: carlosdelfino
https://avatars2.githubusercontent.com/u/369056?s=400&u=c14f3f3c66671fc57e96960ac53329c1d0e5e86f&v=4

Love programming, love get new knowledgement, love to learn. First coded at
age of 13 years old and, since that time, is continously learning and
getting new challenges.

*Paulo Matias*
github: thotypous
https://avatars3.githubusercontent.com/u/262047?s=460&u=fec77dd968decd063a2efae5cfd3d886c5ff0433&v=4



Assistant Professor at DC-UFSCar. Ph.D. in Computational Physics from
IFSC-USP.

*Marcelo Samsoniuk*
github: samsoniuk
https://avatars2.githubusercontent.com/u/42520878?s=460&u=dca55185ec98dbfa6323301d9c1706f45e397323&v=4

Ancient wizard from the 68000-era and maintainer of old opensource projects. 
Currently R&D Consultant and Digital Expert at Unify/Atos, as well
maintainer of the opensource DarkRISCV processor.
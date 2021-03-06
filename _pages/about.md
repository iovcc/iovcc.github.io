---
permalink: /about/
title: "About"
modified: 2020-07-25 
toc: false
author_profile: false
sidebar: false
read_time: true
comments: true
share: true
feature_row:
  - title: "Paulo Matias"
    image_path: "/assets/images/thotypous.png" 
    excerpt: "Assistant Professor at DC-UFSCar.  Ph.D.  in Computational Physics from IFSC-USP. github: thotypous"
  - title: "Marcelo Samsoniuk"
    image_path: "../assets/images/samsoniuk.png"
    excerpt: "Ancient wizard from the 68000-era and maintainer of old opensource projects.  Currently R&D Consultant and Digital Expert at Unify/Atos, as well maintainer of the opensource DarkRISCV processor. github:samsoniuk"
    url: "http://darklife.com"
    btn_label: "Darklife"
    btn_class: "btn--primary"
---

{% include base_path %} 

## About the IO/VCC

The IO/VCC was created in Jul 2020 by Marcelo Samsoniuk and
Paulo Mathias after the analysis of a very weird segment of Verilog code:

```
case(1'b1)
  RST: Q <= 1'b1;
  SET: Q <= 1'b0;
  default: Q <= D;
endcase
```

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

## About the IO/VCC Founders


{% include feature_row %}

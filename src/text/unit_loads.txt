



________________________________________________________________________________

 Load Combinations                                                   0102 - [01]
________________________________________________________________________________

CBC Load Notations                                           [Table: 0102.01.01]
==========  ==============================  =============================
 Notation            Load Effect                        Notes
==========  ==============================  =============================
    D                 Dead load             See IBC 1606 and Chapter 3 of
                                                  this publication
    E       Combined effect of horizontal   See IBC 1613, ASCE/SEI 12.4.2
               and vertical earthquake-         and Chapter 6 of this
             induced forces as defined in            publication
                   ASCE/SEI 12.4.2
    Em      Maximum seismic load effect of  See IBC 1613, ASCE/SEI 12.4.3
            horizontal and vertical forces      and Chapter 6 of this
               as set forth in ASCE/SEI              publication
                        12.4.3
    H         Load due to lateral earth     See IBC 1610 for soil lateral
               pressures, ground water                  loads
             pressure or pressure of bulk
                      materials
    L        Live load, except roof live    See IBC 1607 and Chapter 3 of
            load, including any permitted         this publication
                 live load reduction
    Li       Roof live load including any   See IBC 1607 and Chapter 3 of
            permitted live load reduction         this publication
    R                 Rain load             See IBC 1611 and Chapter 3 of
                                                  this publication
    W         Load due to wind pressure     See IBC 1609 and Chapter 5 of
                                                  this publication
==========  ==============================  =============================

CBC Load combinations                                        [Table: 0102.01.02]
====================  =====================================================
 CBC 2019 reference                          Equation
====================  =====================================================
   Equation 16-1                            1.4(D +F)
   Equation 16-2                 1.2(D + F) + l.6(L + H) + 0.5(L
   Equation 16-3      1.2(D + F) + l.6(Lr or S or R) + l.6H + (f1L or 0.5W)
   Equation 16-4        1.2(D + F) + 1.0W + f1L +1.6H + 0.5(Lr or S or R)
   Equation 16-5              1.2(D + F) + 1.0E + f1L + l.6H + f2S
   Equation 16-6                        0.9D+ l.0W+ l.6H
   Equation 16-7                     0.9(D + F) + 1.0E+ l.6H
====================  =====================================================



________________________________________________________________________________

 Gravity Loads and Mass                                              0102 - [02]
________________________________________________________________________________


Roof unit dead loads                                         [Table: 0102.02.01]
==========  =======  =========  =================================
variable      value    [value]  description
==========  =======  =========  =================================
ld1         2.0 psf  0.096 KPa  Urethane foam (4 inch thick)
ld2         1.0 psf  0.048 KPa  Three-ply roofing
ld3         5.0 psf  0.239 KPa  Doug Fir decking 2-in.
ld4         1.0 psf  0.048 KPa  Doug Fir beams 4x12 at 12 ft o.c.
---------
roofdl1     9.0 psf  0.431 KPa  Total roof unit load
==========  =======  =========  =================================

Floor unit dead loads                                        [Table: 0102.02.02]
==========  ========  =========  ==========================
variable       value    [value]  description
==========  ========  =========  ==========================
ld1          3.0 psf  0.144 KPa  3/4 in. hardwood flooring
ld2          2.0 psf  0.096 KPa  1/2 in. plywood subfloor
ld3          4.0 psf  0.192 KPa  2x10 joists at 16 in. o.c.
ld4          1.5 psf  0.072 KPa  fixtures
---------
floordl1    10.5 psf  0.503 KPa  Total floor unit load
==========  ========  =========  ==========================

Interior wall unit dead loads                                [Table: 0102.02.03]
==========  =======  =========  =============================
variable      value    [value]  description
==========  =======  =========  =============================
ld1         5.5 psf  0.263 KPa  5/8" sheet rock (2)
ld2           2 psf  0.096 KPa  2x4 studs at 16" o.c.
ld3         1.5 psf  0.072 KPa  fixtures
---------
intwalldl1    9 psf  0.431 KPa  Total interior wall unit load
==========  =======  =========  =============================

Exterior wall unit dead loads                                [Table: 0102.02.04]
==========  =======  =========  =============================
variable      value    [value]  description
==========  =======  =========  =============================
ld1         2.0 psf  0.096 KPa  1/2 in plywood sheathing
ld2         2.0 psf  0.096 KPa  2x4 studs at 16 in o.c.
ld3         3.0 psf  0.144 KPa  5/8 in sheet rock
ld4         1.5 psf  0.072 KPa  fixtures
---------
extwalldl1  8.5 psf  0.407 KPa  Total exterior wall unit load
==========  =======  =========  =============================

Building geometry                                            [Table: 0102.02.05]
==========  =======  ==========  ======================
variable      value     [value]  description
==========  =======  ==========  ======================
arearf1     1700 sf  157.935 m2  roof area
areaflr1    1200 sf  111.484 m2  floor area
htwall1        9 ft     2.743 m  wall height
lenwall1     110 ft    33.528 m  interior wall length
lenwall2     155 ft    47.244 m  exterior wall length 2
==========  =======  ==========  ======================
 
                                                roof weight [ Equ: 0102.02.01 ]

rfwt₁ = arearf₁⋅roofdl₁
===========  =========  =========  ===========
   rfwt1      [rfwt1]    roofdl1     arearf1
===========  =========  =========  ===========
15300.0 lbs  68.058 KN  9.000 psf  1700.000 sf
===========  =========  =========  ===========

                                               floor weight [ Equ: 0102.02.02 ]

flrwt₁ = areaflr₁⋅floordl₁
===========  ==========  ==========  ===========
  flrwt1      [flrwt1]    floordl1    areaflr1
===========  ==========  ==========  ===========
12600.0 lbs  56.048 KN   10.500 psf  1200.000 sf
===========  ==========  ==========  ===========

                                           partition weight [ Equ: 0102.02.03 ]

partwt₁ = htwall₁⋅intwalldl₁⋅lenwall₁
==========  ===========  ============  =========  ==========
 partwt1     [partwt1]    intwalldl1    htwall1    lenwall1
==========  ===========  ============  =========  ==========
8910.0 lbs   39.634 KN    9.000 psf    9.000 ft   110.000 ft
==========  ===========  ============  =========  ==========

                                       exterior wall weight [ Equ: 0102.02.04 ]

xwallwt₁ = extwalldl₁⋅htwall₁⋅lenwall₂
===========  ============  ==========  ============  =========
 xwallwt1     [xwallwt1]    lenwall2    extwalldl1    htwall1
===========  ============  ==========  ============  =========
11857.5 lbs   52.745 KN    155.000 ft   8.500 psf    9.000 ft
===========  ============  ==========  ============  =========

                                      TOTAL BUILDING WEIGHT [ Equ: 0102.02.05 ]

totwt₁ = flrwt₁ + partwt₁ + rfwt₁ + xwallwt₁
===========  ==========  =================  ================  ================  ================
  totwt1      [totwt1]       xwallwt1            rfwt1            partwt1            flrwt1
===========  ==========  =================  ================  ================  ================
48667.5 lbs  216.484 KN  11857.500 ft2 psf  15300.000 psf sf  8910.000 ft2 psf  12600.000 psf sf
===========  ==========  =================  ================  ================  ================



________________________________________________________________________________

 Material Densities                                                  0102 - [03]
________________________________________________________________________________

Because the T&G roof is flexible [#]_ , for seismic models calculate the
effective floor load as the sum of the floor and 100%
of the partition weight.

                            floor load including partitions [ Equ: 0102.03.01 ]

          flrwt₁ + partwt₁
eflrdl₁ = ────────────────
              areaflr₁    
==========  ===========  ===========  ================  ================
 eflrdl1     [eflrdl1]    areaflr1        partwt1            flrwt1
==========  ===========  ===========  ================  ================
17.925 psf   0.858 KPa   1200.000 sf  8910.000 ft2 psf  12600.000 psf sf
==========  ===========  ===========  ================  ================

               effective floor density including partitions [ Equ: 0102.03.02 ]

            eflrdl₁
eflrdens₁ = ───────
             0.5⋅IN
=======================  =============  ==========  ====
       eflrdens1          [eflrdens1]    eflrdl1     IN
=======================  =============  ==========  ====
0.24895833080391674 pci  67.579 KN m-3  17.925 psf   in
=======================  =============  ==========  ====

                          effective roof density 1-1/2" T&G [ Equ: 0102.03.03 ]

           roofdl₁
erfdens₁ = ───────
            1.5⋅IN
========================  =============  =========  ====
        erfdens1           [erfdens1]     roofdl1    IN
========================  =============  =========  ====
0.041666666243333345 pci  11.310 KN m-3  9.000 psf   in
========================  =============  =========  ====

                      effective wall density 1/2" sheathing [ Equ: 0102.03.04 ]

             extwalldl₁
ewalldens₁ = ──────────
               0.5⋅IN  
=======================  ==============  ============  ====
      ewalldens1          [ewalldens1]    extwalldl1    IN
=======================  ==============  ============  ====
0.11805555435611113 pci  32.046 KN m-3    8.500 psf     in
=======================  ==============  ============  ====





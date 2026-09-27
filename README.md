# Fonte Linear 12V / 1.5A - LM317K + TIP41 - 11.9V Validada

**Vin 23.5V | Vout 11.9V | Iout 1.49A em 8R | 60Hz | C1 22000uF**

Projeto debugado de 0.17V até 11.9V no Proteus.

## Esquemático Final
Upload do seu print final aqui: FonteLinearAjustavel0-12V.PNG

## Ligação 
VIN -> C1+/C2+/VI p3/Coletor TIP41/Catodo D1
VO p1 -> Base TIP41 + R3 ESQ 1R
VOUT -> Emissor TIP41 + R3 DIR + R1 DIR 240R + Anodo D1 + C4/C5/R2 8R
ADJ p2 -> R1 ESQ + RV1 TOPO + RV1 WIPER + C3+
GND UNICO -> C1-/C2-/C3-/RV1 base/C4-/C5-/R2-/BR2-

Com booster: VOUT = 0.60 * (R1+RV1)/R1
5k = 13.1V -> ajustado 11.9V a 100%


## BOM
KBU4A, 22000uF 35V, 100nF, LM317K, 1N4007, TIP41, 1R 2W, 240R, 5k trimpot, 10uF, 100uF, 100nF, 8R 20W, VSINE 22Vpk 60Hz

## Cálculos
Ripple = 1.5/(120*0.022)=0.56V | P_TIP41=(23.5-11.9)*1.49=17.4W dissipador obrigatório

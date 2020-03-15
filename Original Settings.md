# Artillery Genius factory firmware settings


## Original firmware defaults

```
>>> M503
SENDING:M503
echo:  G21    ; (mm)
echo:Filament settings: Disabled
echo:  M200 D1.75
echo:  M200 D0
echo:Steps per unit:
echo:  M92 X80.12 Y80.12 Z399.78 E445.00
echo:Maximum feedrates (units/s):
echo:  M203 X300.00 Y300.00 Z50.00 E40.00
echo:Maximum Acceleration (units/s2):
echo:  M201 X2000 Y2000 Z100 E10000
echo:Acceleration (units/s2): P<print_accel> R<retract_accel> T<travel_accel>
echo:  M204 P800.00 R10000.00 T2000.00
echo:Advanced: Q<min_segment_time_us> S<min_feedrate> T<min_travel_feedrate> X<max_x_jerk> Y<max_y_jerk> Z<max_z_jerk> E<max_e_jerk>
echo:  M205 Q20000 S0.00 T0.00 X8.00 Y8.00 Z0.30 E5.00
echo:Home offset:
echo:  M206 X0.00 Y0.00 Z0.00
echo:PID settings:
echo:  M301 P9.31 I0.57 D37.76
echo:  M304 P92.46 I16.12 D132.55
```

## Some of my presets

I use them in Filament -> Custom G-code

```
;M301 P11.91 I0.89 D39.75        ; Hotend PID autotuning value 230C fan 100%
;M301 P12.98 I0.98 D42.78        ; Hotend PID autotuning value 225C fan 100%
;M301 P13.27 I1.00 D44.02        ; Hotend PID autotuning value 225C fan 50%
;M304 P85.86 I15.19 D121.33      ; Bed PID autotuning value 60C
;M304 P138.69 I27.30 D176.12     ; Bed PID autotuning value 90C
```

## New defaults

```
echo:Marlin 1.1.9
echo: Last Updated: 2018-08-01 | Author: (kind3r)
echo:Compiled: Mar 14 2020
echo: Free Memory: 4637  PlannerBufferBytes: 1664
echo:V55 stored settings retrieved (655 bytes; crc 9928)
echo:  G21    ; (mm)
echo:Filament settings: Disabled
echo:  M200 D1.75
echo:  M200 D0
echo:Steps per unit:
echo:  M92 X80.12 Y80.12 Z399.78 E445.00
echo:Maximum feedrates (units/s):
echo:  M203 X200.00 Y200.00 Z20.00 E40.00
echo:Maximum Acceleration (units/s2):
echo:  M201 X2000 Y2000 Z500 E5000
echo:Acceleration (units/s2): P<print_accel> R<retract_accel> T<travel_accel>
echo:  M204 P500.00 R10000.00 T500.00
echo:Advanced: Q<min_segment_time_us> S<min_feedrate> T<min_travel_feedrate> X<max_x_jerk> Y<max_y_jerk> Z<max_z_jerk> E<max_e_jerk>
echo:  M205 Q20000 S0.00 T0.00 X7.00 Y7.00 Z0.20 E3.00
echo:Home offset:
echo:  M206 X0.00 Y0.00 Z0.00
echo:Auto Bed Leveling:
echo:  M420 S0 Z0.00
echo:  G29 W I0 J0 Z0.01348
echo:  G29 W I1 J0 Z-0.05906
echo:  G29 W I2 J0 Z-0.01404
echo:  G29 W I0 J1 Z0.07601
echo:  G29 W I1 J1 Z-0.01904
echo:  G29 W I2 J1 Z0.06101
echo:  G29 W I0 J2 Z0.04600
echo:  G29 W I1 J2 Z-0.06656
echo:  G29 W I2 J2 Z-0.02904
echo:PID settings:
echo:  M301 P13.27 I1.00 D44.02
echo:  M304 P138.69 I27.30 D176.12
echo:Z-Probe Offset (mm):
echo:  M851 Z-1.74
echo:Linear Advance:
echo:  M900 K0.00
```
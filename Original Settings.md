# Artillery Genius factory firmware settings

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
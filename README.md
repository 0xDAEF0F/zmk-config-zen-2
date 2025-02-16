Macro syntax:

```keymap
        macros {
                ZMK_MACRO(alacritty,
                        wait-ms = <20>;
                        tap-ms = <30>;
                        bindings
                        = <&kp LG(SPACE)>
                        , <&kp A &kp L &kp A &kp C &kp R>
                        , <&macro_wait_time 120>
                        , <&kp ENTER>
                        ;
                )
        };
```

Tap Dance:

```keymap
        behaviors {
                td0: tap_dance_0 {
                        compatible = "zmk,behavior-tap-dance";
                        #binding-cells = <0>;
                        tapping-term-ms = <300>;
                        bindings = <&kp N>, <&to 1>;
                };
        };
```

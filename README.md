CAN_RA6T2.7z
 ## What it does

  1. Opens CANFD channel 0.
  2. Transitions to **Internal Loopback** test mode.
  3. Transmits a single 8-byte standard CAN frame (ID
   `0x20`) with payload `AA BB CC DD 11 22 33 44`.
  4. Waits for TX-complete and RX-complete callbacks.
  5. Hits a software breakpoint — inspect
  `g_can_rx_frame` in the debugger to verify
  loopback.

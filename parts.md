| Item              | Per-robot Quantity             | Notes                                                           |
|-------------------|--------------------------------|-----------------------------------------------------------------|
| Arduino Uno       | 1                              |                                                                 |
| Status LED        | 6                              | Controller state (3); Color sensor (2); Proximity sensor (1)    |
| Motor shield      | 2                              |                                                                 |
| Large motor       | 2                              | For the wheels                                                  |
| Small motor       | 1                              | For moving the gate                                             |
| Ultrasonic sensor | 2                              |                                                                 |
| Long IR sensor    | 1                              |                                                                 |
| Phototransistor   | 2                              | For color sensing                                               |
| Fixed resistor    | requires further consideration | For converting the phototransistor characteristics to a voltage |
| Dual comparator   | 1                              | For digitizing the color sensors                                |
| Potentiometer     | 2                              | For trimming the color sensor threshold                         |
| Fixed resistor    | 2                              | The other half of the comparator reference voltage divider      |
| Bypass capacior   | requires further consideration | There will be significant motor noise to consider               |
| Main PCB          | 1                              | Contains status LEDs and any other required electronics         |
| Ultrasonic PCB    | 2                              | Adapts ultrasonic connector, as the default looks unreliable    |
| Color sensor PCB  | 2                              | Contains comparators and potentiometer voltage reference        |
| Battery pack      | 1                              |                                                                 |
| Misc connectors   | requires further consideration |                                                                 |

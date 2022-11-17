# CS3103 Programming Assignment

#### Prereqs:
- Python 3 (ensure that python3 is in PATH)

#### Running the program:

To read usage: `./proxy`
``` bash
usage: ./proxy port [img_substitution] [attack_mode]
  port:              the port proxy is listening on
  img_substitution:  set to 1 to replace all imgs
  attack_mode:       set to 1 to turnon attack_mode
```

- Running proxy on port 3000: `./proxy 3000`
- Running proxy on port 3000 with image substitution: `./proxy 3000 1`
- Running proxy on port 3000 with attack mode: `./proxy 3000 0 1`

### Note about telemetry
Since the specifications of the assignment is unclear, my implementation of telemetry is calculated using the entire response message including the http headers.

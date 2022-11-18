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
Telemetry size is not inclusive of header and only limited to the size of the object being passed through the proxy. For requests with content-length, it will
be equal to the number in content-length while in chunked encoding, itll be equal to the total sum of all chunks not inclusive of the chunk size.

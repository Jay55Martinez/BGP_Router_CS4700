# BGP_ROUTER_CS4700

## Overview

BGP_ROUTER_CS4700 is a Python model that simulates a BGP router. It implements essential functions of a real router, such as accepting route announcements, generating new routes, managing a forwarding table, and forwarding data packets from simulated internet users.

## Usage

To run the router, use the command:

    ./4700router <asn> <port-ip.add.re.ss-[peer,prov,cust]> [port-ip.add.re.ss-[peer,prov,cust]] ...

Or with a config file:

    user@host$ ./run configs/<config-file>

## Challenges

1. **Determining if Networks Are Adjacent**: Had to revise the `are_adjacent` method multiple times due to edge cases that caused it to fail.
  
2. **Deaggregation**: Faced difficulties in rebuilding the forwarding table from past messages, often resulting in too many elements remaining in the table.

## Testing and Debugging

Tested by executing various configurations to ensure functionality.
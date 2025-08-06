# Routing Table Comparison: R1 vs. R2

This report summarizes the differences between the routing tables of devices R1 and R2.

## Common Prefixes

The following prefixes were found in both R1 and R2:
*   `1.1.1.0/24`
*   `10.10.10.0/24`
*   `20.20.20.0/24`

## Prefixes Unique to R1

The following prefixes were found only in the routing table of R1:
*   `1.1.1.1/32`
*   `10.10.10.100/32`

## Prefixes Unique to R2

The following prefixes were found only in the routing table of R2:
*   `1.1.1.2/32`
*   `20.20.20.100/32`

## Protocol Differences

Interestingly, two of the common prefixes were learned via different routing protocols on each device:
*   **10.10.10.0/24:** Connected on R1, Static on R2.
*   **20.20.20.0/24:** Static on R1, Connected on R2.

This indicates a difference in the network configuration and how these networks are attached to each router.

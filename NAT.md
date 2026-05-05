# NAT Basics

## What I learned today

Today I learned about **NAT**, which stands for **Network Address Translation**.

NAT is used by routers to let devices inside a private network communicate with the internet.

## Simple explanation

My home devices have **private IP addresses**.

Example:

- Laptop: `192.168.1.10`
- Phone: `192.168.1.11`
- Printer: `192.168.1.12`

These private IPs work inside my home network, but they are not used directly on the public internet.

When my laptop goes to a website, the router changes my laptop’s private IP into the router’s public IP.

That is NAT.

## Mental picture

NAT is like a front desk at a hotel.

The people inside the hotel have room numbers.

The outside world does not talk directly to each room.

Instead, the outside world talks to the front desk.

The front desk knows which room asked for what and sends the response back to the correct room.

In networking:

- Private device = hotel room
- Router = front desk
- Public IP = hotel’s main address
- NAT table = front desk notes

## Why NAT matters

NAT matters because it allows many devices to share one public IP address.

Without NAT, every device would need its own public internet IP address.

## Quick example

My laptop sends traffic to a website.

The router changes:

```text
From: 192.168.1.10
To: Public IP address

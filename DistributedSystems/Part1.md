# Part 1

## Direct Communication (chapter 4,5,8)

Direct: if the sender and receiver are aware of each other

note: chapter 3 helicopter view (Assumed to be known)
  1. Intro (concepts, terms)
  2. Types of network (LAN, WAN,...)
  3. Network principles: packet transmission, data streaming, switching, protocols, routing, congestion control,...
  4. Internet protocols: IP addressing, IP routing, IPv6,....
  5. case studies: Ethernet, WiFi and Bluetooth
  6. Summary

TCP is more reliable, but more costly, UDP less reliable, but cheaper => OS level, but example of impact of choices.

chapter 4: helicopter view
  1. Intro
  2. the API for the internet protocols (Assumed to be known)
  3. External data representation and marshalling (serialization / de-serialization => assembling/disassembling data in order to transmit it)
  4. Multicast communication (skipped)
  5. Network visualization : Overlay networks (skipped)
  6. Case study: MPI (skipped)
  7. Summary

### Introduction
Communication: data representation?
Synchronization: (how to express cooperation?) who is waiting for who?

Important: although we do not meddle with the lower layers, we have to be aware of it: ex. choice of protocol, what happens if packet gets lost?

Distribution service middleware (see slide 6)
  - shields developers of a distributed application from the complex distributed environment (low level socket API, No transfer of structured data,..)

#### Data representation:
Problem:
  - program data: typed, structured, object
  - message data: bit/byte streaming
  - different representations of data in heterogeneous systems (32 bit vs 64 bit,....)

Conversion: different approaches:
  - agreed form for transmission (for example with a standard like Sun NFS)
  - full data description transmission (type, length, value coding on the wire, interpretation at receiving site possible => slower)
  - Conversion to ASCII text (ex. XML)

#### Message passing:
  - Procedure sender
  - Procedure receiver
  - Synchronous vs asynchronous

#### Message destinations:
  - message destination = communication identifier (preference for location independent identifiers)
  - can be of different types: port, machine,...

#### Message reliability:
  - possible failures (corrupted messages, duplicates, order,...)
  - reliable communication (delivered uncorrupted, in order, without duplicates, despite a reasonable number of packets dropped or lost, perfectly reliable communication can not often be guaranteed)


=> To implement reliable communication

Case study: TCP vs UDP (see slide 32-36)
Choice is dependent on application. For ex temperature sensor on Miami beach vs bank app => if duplicates


#### Message conclusion: (see slide 37)

#### Request-Reply Protocols (see slide 38-40)

From data layer, add network layer, then Marshalling, ... until remote procedure calls.

### Remote procedure calls
#### 

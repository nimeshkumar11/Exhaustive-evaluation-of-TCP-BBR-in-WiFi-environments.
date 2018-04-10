# Exhaustive evaluation of TCP BBR in WiFi environments.

## Course Code: CS821

## Assignment: #11

### Overview
Bottleneck Bandwidth and RTT (BBR) [1] is a a new congestion control proposed by Google and has been implemented in Linux. This project aims to evaluate the performance of TCP BBR in wireless networks, especially WiFi.

### Simulation
We here created wireless dumbbell topology to test TCP BBR.

 ``` 
  
    n1                                n5  
      \                              .
       \                           .                    ------ (Point to Point link)
         \                       .                                  
          \                    .
           \                 .                          ...... (Wireless link)
n2 -------- n4------------- AP. . . . . n6
          /                  .
         /                     .                        Here, in this example AP is a wireless device, and 
        /                        .                         n4, n5, n6 are station nodes        
       /                           .
      /                              .
   n3                                   n7    
                                              
                                            
```
### References

[1] [Neal Cardwell, Yuchung Cheng, C. Stephen Gunn, Soheil Hassas Yeganeh, Van Jacobson (2016). BBR: Congestion-Based Congestion Control.](https://queue.acm.org/detail.cfm?id=3022184)

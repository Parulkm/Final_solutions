# Parul Kumawat

## Three major results from the Ranjan et al study
here are the three major results presented in the study:

1)The adaptively coupled mouse brain network model revealed that resource dynamics significantly influence transient explosive synchronization.

2)Network structure played a crucial role in modulating the duration and extent of synchronization events

3)Spatial propagation patterns of synchronization were observed to be influenced by both resource dynamics and network topology, indicating intricate interplay among these factors.

## Key nodes involved in the propagatin of synchronization

List them here

In the paper, several key nodes in the mouse brain are identified as potentially important for the propagation of synchronization. Some of these key nodes include:

1. Hippocampus
2. Thalamus
3. Cortex
4. Striatum
5. Amygdala

## Basic model simulation (single iteration)

### How many transitions do you see in a single simulation run?
Write a single number here. Also include a plot of the entire timeseries.

130 transition
![transition time plot](https://github.com/csndl-iitd/srg-jrf-assignment-template/assets/168579289/c2706930-e3f3-4976-91bb-732772e56b6c)


### How do you define the transition time?
Write the brief description of how you define the transition time.

The transition time, as defined in the provided function compute_transition_times, represents the time instances at which the global order crosses a specified threshold value. More specifically:
1)  It iterates through the global_order array, which contains the global order values at different time points.
2)  At each time point, it checks if the previous global order value is below the specified threshold and the current global order value is equal to or above the threshold.
3)   If this condition is met, it records the time index (i) as a transition time, indicating the time at which the transition from a state below the threshold to a state above the threshold occurs.
   In summary, the transition time represents the discrete time points where a specific condition (crossing a threshold) is met in the time series data (global order values).

### What is the average transition time you observe? Include units!
Write a single number here. You can include a plot that shows all transitions superimposed, aligned to the start time of the transition.
![transition time plot](https://github.com/csndl-iitd/srg-jrf-assignment-template/assets/168579289/1aec6056-1ae9-4277-bbb2-cab4a0e10468)



### Include a box plot of the transition times for a single experiment below.
Include the plot here.

![Box plot of transition time](https://github.com/csndl-iitd/srg-jrf-assignment-template/assets/168579289/23fdd2f1-cd6f-41cd-8960-70f545fc4526)



## Basic model simulation (different initial conditions)

### Include two box plots below, one for number of transitions and another for transition time
Include the plots here.

![box plot number   transitions](https://github.com/csndl-iitd/srg-jrf-assignment-template/assets/168579289/6fb1c9a1-0e16-45de-95e7-1d9a26d7ef8a)


## Advanced simulations

### Box plot for number of events
Include the plot here.


### Box plot for transition time
Include the plot here.

## Interpreting results

Provide your answer here.

Based on the paper's focus on the interplay between resource dynamics, network structure, and spatial propagation of transient explosive synchronization (TES) in an adaptively coupled mouse brain network model, there are several factors that could potentially affect the transition time and number of events. Some of these factors include:
1) Resource Availibility
2) Network Topology
3) Node Properties
4) EXternal Stimuli

   To check the effect of these factors, you could conduct systematic experiments or simulations where you manipulate one factor while keeping others constant. For example:
   
   Resource Availability: Vary the availability of resources in the network and observe how it affects the transition time and number of events. This could involve adjusting parameters related to resource allocation or consumption in the model.

    Network Topology: Generate networks with different topological properties (e.g., random, small-world, scale-free) and analyze how each type of network structure influences synchronization dynamics. You could also selectively remove or add connections to examine their impact.

    Node Properties: Modify the properties of individual nodes (e.g., excitability, threshold) and investigate their effects on synchronization events. This could be done by systematically altering node parameters in the model.

    External Stimuli: Apply external stimuli of varying strengths or timings to the network and assess their effects on synchronization dynamics. This could involve simulating different types of stimuli (e.g., sensory inputs, electrical stimulation) and analyzing their impact on transition times and event frequencies.

By systematically exploring these factors through experiments or simulations, you can gain insights into the complex interplay between resource dynamics, network structure, and external influences on transient explosive synchronization in the brain network model.

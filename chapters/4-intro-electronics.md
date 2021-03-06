## Chapter 4 -- Electronics

Since we're learning all about embedded development, we need to spend some time learning about electronics. How do microcontrollers send information between sensors, displays and other microcontrollers? Electronics is a huge field, and encompasses a large number of topics, so it's impossible for us to cover every topic exhaustively. So, rather than trying to exhaustively cover the field of electronics, what we'll try and do is introduce enough topics that you can put together simple circuits, hook components together and start to understand what is going on with the embedded devices you see around you.

Since there is such a large number of topics to cover, don't worry if this doesn't all make sense on your first readthrough. Most of this is stuff that you will have a chance to learn along the way. But since we can't cover everything in the limited time we have, this section is meant to be a reference to come back to as the program progresses.

### Voltages and Currents



To build any electronic device, we need to have a way of sending signals between controllers, sensors and outputs. The
The way we send those signals is by sending electrons from one place to another, the movement of electrons through is circuit is called *current*.

The way create a current is to apply a *voltage*, a difference in voltage between two points in a circuit will cause current to flow.

So there are two things we want to keep track of in electronic circuits: **voltage** and **current**.

Two things to remember:
* **Voltage is _across_ things**
* **Current flows _through_ things**

The voltage at any point in the circuit generally means **the potential difference between that point and ground**.

### Relating voltage and current: resistors

The current *through* a device is proportional to the voltage *across* it.

This gives us the relationship called Ohm's Law, which is the most important equation in electronics.

![Ohm's Law](https://latex.codecogs.com/svg.latex?V%20%3D%20IR)

The *voltage* is the *resistance* times the *current*.
**Remember this equation!** Seriously. It's the foundation of everything.

### What is resistance?

Like it's name would suggest, it resists current flow. Current can flow much easier through a circuit with lower resistance, but very little current will flow in a circuit with a large resistance. More resistance, less electrons flowing. The unit of resistance is an ohm (Ω).

### Series and parallel

Resistors in series look like this:

![Resistors](https://upload.wikimedia.org/wikipedia/commons/1/11/Resistors_in_series.svg)

To total resistance is just the sum of their resistances together.

![Resistors in series](https://latex.codecogs.com/svg.latex?R_%7Btot%7D%20%3D%20R_1%20&plus;%20R_2%20&plus;%20...%20&plus;%20R_n)

So when something is *in series*, it means that the only way for current to flow is through the device.

When something is in *parallel*, it means there are *multiple paths for current to flow*.

So parallel resistors look like this:

![Parallel resistors](https://upload.wikimedia.org/wikipedia/commons/0/09/Resistors_in_parallel.svg)

The equation, if you care about that sort of thing....

![Parallel equation](https://latex.codecogs.com/svg.latex?R_%7Btot%7D%20%3D%20%5Cfrac%7B1%7D%7B%5Cfrac%7B1%7D%7BR_1%7D%20&plus;%20%5Cfrac%7B1%7D%7BR_2%7D%20&plus;%20...%20&plus;%20%5Cfrac%7B1%7D%7BR_n%7D%7D)


## Analog and Digital

**Analog** (should be analogue but we're lazy) deals with *continuous* values, or *ranges of values*. So when we want to measure ranges of things, it will generally be an analog circuit.

**Digital** circuits are either *on* or *off*. We don't do ranges anymore, it's a binary world. On or off. 0s or 1s. That's it.

The world is in analog, and digital is us making constraints on it. So if it's a thing like "pressing a button" or "turning on a light", it's digital. If we're *measuring a range*, it's analog.

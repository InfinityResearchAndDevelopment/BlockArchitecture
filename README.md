# BlockArchitecture
The BlockArchitecture is a computer architecture that contrasts from binary in that instead of having a base of 2, the BlockArchitecture utilizes a proprietary protocol called VAT, or Voltage Amplitude Translation, which has a base of 18.

:VAT
-VAT's scales are as follows ~,0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F,N
-VAT is essentially hexadecimal represented on the line level, with two more control bits added.
~, is equivelant to NULL, 0 volts, ground. But ~ does not represent the number 0 as compared to tradition, being that 0 is still a number abliet essentially hollow.
N, would equivelant to Source, V++, Infinity, basically the rail's max potential.
In the origional theory, VAT did not contain ~, only N, which was an interrupt at the time.

:BlockArchetecture
The BlockArchitecture is the syntax, or the way that VAT is implemented into a framework, it is the basis for development, like assembly in tradtional computing.  In VAT the elements ~, and N both act as dynamic interrupts which are scope-sensitive. They are both used to switch contexts of execution, make jumps, calls, both blocking or nonblocking execution can be implemented. This architecture has dynamic precision, meaning it can switch context with exponentional precision on the fly.

The base theory of the BlockArchitecture has a starting precision of 4, that is 4 bits of data per instruction DEAD BEEF would be two SubBlocks.

The original theory process in Blocks, which consisted of 16 SubBlocks, a header, two parameters, and a return, or forward segment.
THe Block was formatted as follows:
CPU,Function,SubFunction,ExpectedDataFormat <Header>
UnDef,UnDef,UnDef,UnDef <Parameter1>, always used the same space, and the space of the parameters can be partitioned as desired.
UnDef,UnDef,UnDef,UnDef <Parameter2>
<Return/Fwd>, (CPU,Function,SubFunction,ExpectedDataFormat)

Essentially acting as a neural network in that blocks can conatin information, and or what to do with it.
Again, this was the original theory wich was riddled with issues, so the current thepry has differed somewhat.

:BlockGeneration
Think about inverse Ansestry and exponets. Binary would be considered a BlockGeneration or a BlockGen of 2, having the equivelent of 1 binary byte. or a base of 2 VAT bits. BlockGen can be anywhere between 1, and infinity follow the follow convention:
1,2,4,8,16,32,64,128,etc up to infinity (theoretically of course) The limitation being the VAT Bus width, or physical bus lines.

Having a base of 18, 1 BlockGen has of course 18 possible values, and exponentionally grows proportionately with the BlockGeneration in context. Consider the BlockGen of 4 as is the default, along with the standard Block Header.

The first call in the system at any interrupt is the CPU, then the Function within that CPU, and the Subordinate Function within the function of that CPU. The Gateway is always 0,00,0000,00000000, etc. Now lets throw some theoritical limits for the addressing scheme out:
18^4=104,976 Total addressable CPUs
104,976 CPUs=121,439,531,096,594,251,776 Total addressable functions
and the limits go higher with respect to the BlockGen.

By default the system will consist of application specific coprocessors starting with the Gateway, its purpose is similar to the traditional CPU in that is traffics information and streamlines a default set of integrated functions.

To be continued...

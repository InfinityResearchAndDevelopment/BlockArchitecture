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

By default the system will consist of application specific coprocessors starting with the Gateway, its purpose is similar to the traditional CPU in that it traffics information and streamlines a default set of integrated functions.

:GhostIO
Traditionally when a bit of data is erased, it is either ignored or overwritten. In this case, values are literally recycled in contrast to the recycle bin in window's operating systems. With GhostIO there is an input and an output, essentially being the equivelant of nul and rand, but in this case when data is sent to nul it is pooled along with other sources such as the Random Signal Generator. All input is osbfuscated and perplexed the result is a feedback loop between Nul and Rand or the Input and Output of the GhostIO, resulting in true noise. Each CPU will contain its own unique RandomSignalGenerator and the output will be pooled along with the other sources in the Gateway's GhostIO. Each CPU can either pull Infinity from either the central GhostIO or via it's own internal source but not of that elsewhere. The idea of having a central pool for infinity and localized counter points is to bring out a better reference points of entropy via different points in space/time. Not 100% nessicary at the current stage of development, but in the future it will be essential in terms of AI.

:Initialization process
THe the machine is first powered up the Gateway and all coprocessors will put themselves in an idle listening state. The gateway will respond to only BootBlock Functions. Which is called using a simple instruction: 0000.0000.0000.0000, or Gateway.BootBlock.Bootstrap.Default

The Gateway then initializes its internals, and finally the VAT Bus. The Gateway then requests the CPUs to init themselves by sending them the bootstrap instruction, when the CPU beings to stream its RSG the GhostIO will initialize a feedback loop of noise to the CPU.
At this point the CPU is idle and ready.

:The Gateway
The gateway provides the basic functionality to implement an operating system such as BlockOS which would be equivelant to BIOS/UEFI in traditional-modern systems.
The Gateway has several internal functions such as arithmitec, cache, volatale, and non-volitale storage.
0000.BootBlock
0001.Query
0002.Math
0003.VS
0004.NVS
0005.GhostIO
0006.vCPU
etc...
Now these functions are alpha and merely serve as an example, but the order, and the number of base functions has yet to be determined.

VirtualCPUs:
The gateway has the ability to define and process 16 unique software processors, each with their own RSG in addition to the others.
Each psyhical CPU can either be a 100% firmware blank, or be an application-specifically designed one.
This is where the vCPUs come in. A vCPU will act just like a physical one. For example, an x86 VM operating in BlockGen 2 could be implemented operating like an Intel processor. vCPUs can be used for development in production CPU models as well. The concept behind such a system would appear to be a never before seen computer architecture, setup, and layout, and run your favorite distro, or even windows but also be able to handle massive throughput due to operating on a Base 18 processor rather than a binary one.

:Other
Another point to add is the clock speed, the rate at which such a system could transfer data is exponentional due to the density of data that can be represented in a single unit.

To be continued...

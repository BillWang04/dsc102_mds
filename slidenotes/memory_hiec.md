# Memory Hiearchy 

**Processor**: Hardware to orchestrate and execute instructions to manipulate data as specified by a program.
- The processor loads memory and instructions into the processor
- specifies bit length/format of machine code commands

**Registers**: are tiny memory in processor where instructions and data are copied to.

**Processing the Data:** There are Different types of ISA commands for each processor
- Memory Access: LOAD(Loading data from DRAM into register), STORE(Putting data into DRAM)
- Arithmetic Access: on data items in registers:
add/multiply/etc.; bitwise ops; compare, etc.; handled by ALU
- Control flow (branch, call, etc.); handled by CU

OOM MEANS MEANS OUT OF MEMORY NOT OUT OF MANA

How Processing Works:

Fetch Instructions (check instruction pointer and load instructions into processor) -> Decode Instruction (Checks what operations need to be done) -> Fetch Data ( obtaining operands or data required by the instruction directly from internal CPU resources, such as registers or caches) -> Execute Instruction(Do the operations) ->  Memory Access (Interact with Dram) -> Write results back into memory -> Next Instructions -> Next Instruction (check pointer for next instruction)

Caches: Small local memory to buffer  instructions/data (basically temporary storage from moving one place to another and so future steps may use)


**Concepts of Memory Management**
- Caching: Buffering a copy of bytes (instructions and/or data)
from a lower level at a higher level to exploit locality
- Prefetching: Preemptively retrieving bytes (typically data) from
addresses not explicitly asked yet by program
- Spill/Miss/Fault: Data needed for program is not yet available
at a higher level; need to get it from lower level
- Register Spill (register to cache); Cache Miss (cache to
main memory); “Page” Fault (main memory to disk)
- Hit: Data needed is already available at higher level
- Cache Replacement Policy: When new data needs to be
loaded to higher level, which old data to evict to make room? Many policies exist with different properties'

**Difference Between Cache and Register**

Cache is a small, high-speed component of a computer system's memory. Registers are fast storage elements integrated into the computer's processor. Cache stores frequently accessed data of a computer. Registers store the data that the CPU is currently processing.


**Example**
- If I want block A in memory, I check cache, if block A in cache, it's a hit
- If not, then its a Miss/Fault/Spill

## Key Principle(Locality of Reference)
- Essentially, when you are accessing DRAM, programs do it in a predictable mannerr
    - Spatial: Nearby locations will be accessed soon
    - Temporal: Same locations accessed again soon
- Exploting these ideas can allow for better optomization. 


$\colorbox{Blue}{Key Principle: Raise cache hits; reduce memory stalls!}$











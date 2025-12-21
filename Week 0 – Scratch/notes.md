# CS50x – Week 0 (Introduction)

## What Computer Science really is

Computer Science is not about learning programming languages.
Languages are just tools.

The core of Computer Science is **problem solving**:

- understanding a problem
- breaking it into smaller parts
- defining clear steps to solve it

This means that learning how to think is more important than memorizing syntax.

## Key idea: Problem Solving

A computer will only do exactly what you tell it to do.
If the instructions are unclear or incomplete, the result will be wrong.

So the real challenge is not coding,
but expressing solutions in a precise and logical way.

## MIT Fire Hydrant Story

One of the examples shown was the famous MIT fire hydrant hack,
where students connected a fire hydrant to a drinking fountain.

 This illustrates:

- creativity in problem solving
- using existing systems in unexpected ways
- thinking beyond the "intended use" of a tool

## Personal interpretation – Learning perspective

I also interpreted this example from a learning perspective.

It shows that having a large **supply of information** is not enough
if the system (or the person) cannot absorb it at the same pace.

In the context of studying:

- consuming too much content at once leads to shallow understanding
- learning requires time to process and reflect
- progress depends on absorption, not volume

This reinforces the importance of studying at a sustainable pace,
focusing on depth rather than speed.

## Binary

Computers represent data using binary numbers (0 and 1).

Each **bi**nary digi**t** represents a power of 2.
By combining bits, computers can represent numbers, text, and instructions.

## ASCII

ASCII is a standard that maps numbers to characters.

By using numeric codes, computers can represent letters, digits,
and symbols using binary values.

This shows that text is not stored as characters,
but as numbers that are interpreted by a standard.

### Numbers vs Characters – Context matters

While studying ASCII, I had a question about how a system
distinguishes a number from a character.

Computers do not inherently know the difference between a number and a character.
They only store binary values.

For example, the value 64 in memory can represent:

- the number 64, if interpreted as an integer
- the character '@', if interpreted using the ASCII standard

The meaning depends on context:

- the data type
- the program logic
- the convention used to interpret the bits

This helped me better understand why typed programming languages exist.
By explicitly defining data types, the language provides context
about how the stored bits should be interpreted.

This shows that data has no meaning by itself.
Meaning comes from how the system interprets it.

## Unicode – A global character system

Unicode exists to solve the limitations of ASCII.

ASCII can only represent a small set of characters,
which is not enough for a world with multiple languages,
symbols, and emojis.

Unicode provides a universal standard that assigns
a unique code point to every character, regardless of:

- language
- platform
- operating system

This allows the same text to be represented consistently
across different systems.

An important realization is that Unicode is not a font.
It is a mapping system that defines *what* a character is,
not *how* it looks.

## Color – Representation and abstraction

Colors in computers are also represented using numbers.

A color is not stored as “red” or “blue”,
but as numeric values that represent intensity.

For example:

- RGB represents colors using red, green, and blue values
- each channel is usually stored as an integer

This reinforces the idea that computers only deal with numbers.
Meaning is created through interpretation and conventions.

From a programming perspective,
this is another example of abstraction:
we work with colors as concepts,
while the system handles numeric representations underneath.

## Representation – Pixels and meaning

While studying representation, I found it interesting how images
are broken down into pixels.

Each pixel is composed of multiple color channels:

- red
- green
- blue

Each channel is usually represented by 8 bits,
which means a single pixel commonly uses 24 bits in total.

This means that an image is essentially a large collection
of numbers arranged in a structured way.

What we perceive as an image:

- shapes
- colors
- depth

is actually the result of numeric representation
combined with interpretation rules.

This reinforced the idea that computers do not store images,
colors, or objects they store numbers.
Everything else is abstraction.

### Audio – Sound as data

Sound is represented digitally by sampling air vibrations.

Instead of storing continuous sound waves,
computers store discrete samples taken at fixed intervals.

Each sample represents:

- the amplitude of the sound wave at a given moment
- stored as a numeric value

The quality of audio depends on:

- sample rate (how many samples per second)
- bit depth (how precise each sample is)

This means that music, like images,
is ultimately a sequence of numbers
interpreted according to agreed standards.

### Video – Images over time

Video can be understood as a sequence of images
displayed rapidly over time.

Each frame is an image composed of pixels,
and each pixel is represented numerically.

Key factors in video representation include:

- resolution (number of pixels per frame)
- frame rate (frames per second)
- color depth

This shows that video is not a fundamentally new concept,
but a combination of:

- image representation
- time

Again, meaning comes from interpretation,
not from the data itself.

## Algorithms – Growth and efficiency

This graph compares how different algorithms scale
as the size of the problem increases.

- O(n): processes one item at a time
- O(n/2): processes more items per step, but still grows linearly
- O(log₂ n): reduces the problem size by half at each step

The key insight is that O(n/2) is still O(n),
because constants do not change how an algorithm scales.

O(log₂ n) is fundamentally different.
Instead of solving the entire problem,
it repeatedly eliminates half of the remaining data.

Using the book example:

- O(n): checking page by page
- O(n/2): checking multiple pages per step
- O(log₂ n): opening the book in the middle and discarding half each time

This explains why logarithmic algorithms scale much better
as the input size grows.

### Binary Search – Dividing the problem

Binary search is an algorithm used to find an element
in a **sorted** list.

Instead of checking each element one by one,
binary search repeatedly divides the search space in half.

The process works as follows:

1. Look at the middle element of the list
2. Compare it with the target value
3. If the target is smaller, discard the right half
4. If the target is larger, discard the left half
5. Repeat until the element is found or the list is empty

Each step removes half of the remaining data.
Because of this, binary search runs in **O(log₂ n)** time.

A practical example is searching for a word in a dictionary:
instead of reading every word,
you open the book in the middle and discard half of the pages
based on alphabetical order.

An important requirement is that the data must be sorted.
Without ordering, binary search cannot be applied.

### Big-O Notation – Measuring algorithm growth

Big-O notation is used to describe how an algorithm
scales as the size of its input increases.

It does not measure actual execution time.
Instead, it focuses on the *growth rate* of the algorithm,
ignoring hardware differences and small constant factors.

Big-O answers the question:
What happens to the algorithm when the input size grows?

Common examples:

- O(1): constant time, input size does not affect performance
- O(n): linear growth, work increases proportionally to input
- O(log n): logarithmic growth, problem size is reduced each step
- O(n²): quadratic growth, common with nested loops

An important rule is that constants do not matter in Big-O:

- O(n/2) → O(n)
- O(2n) → O(n)

This is because Big-O describes long-term behavior,
not small optimizations.

Big-O helps compare algorithms based on scalability,
not speed on a specific machine.

## Pseudocode – Describing logic without syntax

Pseudocode is a way to describe an algorithm
using human-readable steps instead of a real programming language.

It focuses on *logic*, not syntax.
There is no strict standard, and it does not need to compile.

The goal of pseudocode is to:

- think clearly about a solution
- communicate ideas
- plan an algorithm before coding

Because it is language-agnostic,
pseudocode can later be translated into any programming language.

Example of pseudocode logic:

- start
- repeat steps
- make decisions
- stop

Pseudocode helps separate problem solving
from language-specific details.

## Artificial Intelligence – Machines making decisions

Artificial Intelligence (AI) refers to systems
that can perform tasks which normally require human intelligence.

Instead of following fixed instructions,
AI systems often make decisions based on data,
rules, or learned patterns.

At a fundamental level, AI is built on:

- algorithms
- data
- representation
- interpretation

Machine behavior is not “intelligent” by itself.
It is the result of carefully designed logic
combined with large amounts of data.

In many cases, AI systems:

- evaluate possibilities
- assign values or probabilities
- choose the best option based on defined criteria

This reinforces an important idea from computer science:
even complex behaviors emerge from simple rules
applied at scale.

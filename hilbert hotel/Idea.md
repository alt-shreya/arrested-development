As part of the QCHack IBM Quantum Creative challenge. Due to the paucity of time, I couldn't execute it very well.

# Idea
My idea's based on the Hilbert Hotel, or the Infinite Hotel Paradox. The hotel has infinity rooms, which are all occupied. 
The objective of the game I have in mind is to assign rooms at each level. 

## Cases
In the Hilbert's paradox, a few cases are considered, as follows:

- **Case 1:** One person arrives to the hotel. the manager then assigns each current occupant of the (n)th room the (n+1)th room; ie n ---> n+1, and the manager is able to create room.
- **Case 2:** x no. of people arrive at the hotel. The manager assigns each current occupant of the (n)th room the (n+x)th room, ie n ---> n+x.
- **Case 3:** 1 infinitely long bus full of countably infinite people arrives. Then the manager assigns each current occupant of nth room the 2nth room ie, n ---> 2n.
- **Case 4:**  an infinite no. of infinite buses arrive. Manager assigns rooms based on exponents. 

# More Information about Hilbert's Hotel Solution
More information about how he does this can be found from the [solution explanation](https://www.youtube.com/watch?v=Uj3_KqkI9Zo) of the paradox.  
I've also found these blogs helpful: [Part 1](https://medium.com/i-math/hilberts-infinite-hotel-paradox-ca388533f05) | [Part 2](https://medium.com/i-math/infinite-hotel-paradox-continued-f94fe08ec85).

# Employing Quantum
I came across [a paper which shows how you can map a quantum state to 2 or 3 times the quantum state](https://arxiv.org/abs/1506.00675), which I believe is a solution to Case 3. 
In the paper, there is also a mention of the [Sudarsharn-Glogower bare operator that shifts all the amplitudes of the current state up one level](https://arxiv.org/abs/1403.0059) leaving the vacuum state unoccupied - a solution to case 1, and by extension, case 2.
I want to use Qiskit to implement the backend operations of assigning room numbers. 
I think it would be an interesting approach to use Quantum Computers to process infinty.

# Updates to Spec

## 04-21

### Added a Submission Instructions section to reiterate some instructions from previous assignments

### Adding a Project Meeting subsection under Grading
More details and a link to schedule your 10 minute meeting with us during finals week.

### Adding ordering for command-line arguments to the binary
Your binary should take the map as the first argument and the species list as the second.

### Relaxing constriant in Ecosystem Rule 1:
We have now removed the following from rule 1: "Plants get their turn first, then the herbivores, then the omnivores, then the cycle repeats at the next iteration."
This gives you less things to encode when it comes to order of action of organisms.

### Making an implicit constraint explicit in Ecosystem Rule 2:
We have added this to rule 2: "An animal has to move if it can." This was implicitly true but this is just to make things clear.

### Clarification in Ecosystem Rule 6:
We have added this to rule 6: "Furthermore, a plant can't be consumed in a partially grown state." This is a clarification that makes implementation simpler.

### Correction in Ecosystem Rule 11.1:
In rule 11.1, we have changed: "If it sees a predator it moves in the opposite direction, as long as it has more than one unit of energy and space to move." to "If it sees a predator it moves in the opposite direction, as long as it has *at least* one unit of energy and space to move." This removes some ambiguity.

### Making an implicit constraint explicit in Ecosystem Rule 11.2:
In rule 11.1, we have changed "If it sees a prey it moves to consume the prey." to "If it sees a prey **and it can consume it**, it moves to consume the prey." This follows from a previous rule.

### Added compiler requirements to the Compilation and Organization Section:
Added this paragraph:
"You don't need to use FastX to code the project but **make sure** your project builds and runs using the versions of 
Make (`GNU Make 4.4.1`) and g++ (`g++ (GCC) 13.2.1`) that exist in FastX. You can either clone and run your 
repository within FastX to make sure of this, or update your versions to the ones mentioned above. Differences in 
compiler versions lead to weird behaviors sometimes so please ensure compatibility. If your code doesn't compile
with the FastX compiler version, it will be considered as non-compiling (which won't get you too many points)."

### Added sections for External Libraries, Extra Credit and Testing
Also added a new map `map2.txt` that you can test your 
code on.
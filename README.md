# Automatons
A group school to do diffrent operations on automatons
Sure, here's the content for the README file:

# Automata Theory Project

This project is an implementation of various operations and algorithms related to automata theory in the C programming language. It allows you to load automata from text files, perform operations such as union, intersection, and minimization, and generate visualizations of the automata using the DOT language and GraphViz.

## Installation

1. Clone the repository: `git clone https://github.com/your-username/automata-theory.git`
2. Navigate to the project directory: `cd automata-theory`
3. Compile the code: `gcc -o automate final.c`

## Usage

To run the program, execute the following command:

```
./automate
```

This will display the main menu, where you can choose to work with one or two automata:

```
Menu Principal:
1: Operation sur Une automate
2: Operation sur 2 automate
0: Exit
```

### Working with One Automaton

If you choose option 1 (Operation sur Une automate), you will be prompted to enter the name of the text file containing the automaton definition. The file should follow the format:

```
<transition_1>
<transition_2>
...
<transition_n>
<initial_states>
<final_states>
```

Where each `<transition_i>` is a line of the form `<start_state> <end_state> <symbol>`, representing a transition from the start state to the end state with the given symbol. The `<initial_states>` line contains a space-separated list of initial states, and the `<final_states>` line contains a space-separated list of final states.

After loading the automaton, you can perform various operations:

1. **Afficher les alphabets**: Display the alphabet of the automaton.
2. **Generer le fichier dot et afficher l'image png**: Generate the DOT file and display the PNG image of the automaton using GraphViz.
3. **Afficher Tous les etats**: Display all states of the automaton.
4. **Afficher les etats initiaux**: Display the initial states of the automaton.
5. **Afficher les etats finaux**: Display the final states of the automaton.
6. **Tester si un mot est engendré**: Test if a word is accepted by the automaton.
7. **Tester les mots d'un fichier**: Test if the words in a text file are accepted by the automaton.
8. **Etoile de l'automate**: Compute the Kleene star of the automaton.
9. **Supprimer les transitions epsilon**: Remove epsilon transitions from the automaton.
10. **Afficher l'automate deterministe**: Convert the automaton to a deterministic finite automaton (DFA) and display it.
11. **Minimiser automate**: Minimize the automaton using Moore's minimization algorithm.

### Working with Two Automata

If you choose option 2 (Operation sur 2 automate), you will be prompted to enter the names of two text files containing automata definitions in the same format as before.

After loading the two automata, you can perform the following operations:

1. **Union des automates**: Compute the union of the two automata.
2. **Produit des automates**: Compute the product of the two automata.

## Examples

Here are some examples of how to use the program:

1. Load an automaton from a file:

```
Donnez le nom du fichier .txt: demo/example1.txt
```

2. Generate the DOT file and display the PNG image:

```
2: Generer le fichier dot et afficher l'image png
```

This will create a file named `automate.dot` containing the DOT representation of the automaton, and open the corresponding PNG image using GraphViz.

3. Test if a word is accepted by the automaton:

```
6: Tester si un mot est engendré
Entrez le mot à tester: abba
abba est engendré.
```

4. Compute the union of two automata:

```
Donnez le nom du premier fichier .txt: demo/example1.txt
Donnez le nom du deuxieme fichier .txt: demo/example2.txt
1: Union des automates
```

This will display the union automaton and generate the corresponding DOT file and PNG image.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

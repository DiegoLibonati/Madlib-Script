# Madlib-Script

## Getting Started

1. Clone the repository
2. Join to the correct path of the clone
3. Use `python madlib.py` to execute script

## Description

I made a python script that allows to play the madlib. Once we execute the script, we will select a valid option of all the stories that there are to choose and then we will enter the ones that it does not ask for. Once finished entering everything it will show us the text of the story with our modifications.

## Feel free to edit my code

Each function is a storie, and you can create like this:

```
def madlib3():
    noun = input("Enter a noun: ")
    plural_noun = input("Enter a plural noun: ")
    noun_two = input("Enter a noun: ")
    place = input("Enter a place: ")
    adjective = input("Enter a adjective: ")

    print(f"Be kind to your {noun}-footed {plural_noun}.\nFor a duck may be somebody`s {noun_two},\nBe kind to your {plural_noun} in {place}\nWhere the weather is always {adjective}.\nYou may think that this is the {noun},\nWell it is.")
```

If you create a new storie, you need to add this to global dictionary:

```
madlib_dictionary = {"Be kind": madlib1, "Old Macdonald":madlib2, "YOUR STORIE TITLE":madlib3}
```

## Technologies used

1. Python

## Galery

![madlib-script](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/madlib-0.jpg)

![madlib-script](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/madlib-1.jpg)

![madlib-script](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/madlib-2.jpg)

![madlib-script](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/madlib-3.jpg)

## Portfolio Link

`https://diegolibonati.github.io/DiegoLibonatiWeb/#/projects?q=Madlib%20script`

## Video

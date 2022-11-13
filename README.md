# Madlib-Script

## Getting Started

1. Clone the repository
2. Join to the correct path of the clone
3. Use `python madlib.py` to execute script

## Description

I made a python script that allows to play the madlib. Once we execute the script, we will select a valid option of all the stories that there are to choose and then we will enter the ones that it does not ask for. Once finished entering everything it will show us the text of the story with our modifications.

## Technologies used

1. Python

## Galery

![madlib-script](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/madlib-0.jpg)

![madlib-script](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/madlib-1.jpg)

![madlib-script](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/madlib-2.jpg)

![madlib-script](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/madlib-3.jpg)

## Portfolio Link

`https://diegolibonati.github.io/DiegoLibonatiWeb/#/projects?q=Madlib%20Script`

## Video

https://user-images.githubusercontent.com/99032604/198900776-b6ee2027-39b9-4413-8c07-ad16e30c39c8.mp4

## Documentation

If you want to create a new history what you must do is to create a function with the name you want in this case and for this example we will use `madlib2()`. Inside the function we will create variables of type input that will be the names, nouns, adjectives, verbs that we want to add in the history and then we will make a print of that history with the previous variables:

```
def madlib2():

    adjective = input("Enter a adjective: ")
    noun = input("Enter a noun: ")
    noise = input("Enter a noise: ")
    animal = input("Enter an animal: ")

    print(f"{adjective} Macdonald had a {noun}, E-I-E-I-O\n \
    and on that {noun} he had an {animal}, E-I-E-I-O\n \
    with a {noise} {noise} here\n \
    and a {noise} {noise}there,\n \
    here a {noise}, there a {noise},\n \
    everywhere a{ noise} {noise},\n \
    {adjective} Macdonald had a {noun}, E-I-E-I-O.")
```

Then what we are going to do is to add that new function to our `madlib_dictionary`. We will pass a key with its name and a value with the function we created in this case `madlib2`:

```
madlib_dictionary = {"Be kind": madlib1, "Old Macdonald":madlib2}
```

Finally we will be asked which book we want to use to play in the form of an index. We will choose a number from the available options and then it will look for the option we passed to the dictionary. Now we will be able to play:

```
for index,title in enumerate(madlib_dictionary.keys()):
    print(f"{index}) {title}")

opcion = int(input("Your selection: "))

for index,title in enumerate(madlib_dictionary.keys()):
    if opcion == index:
        madlib_dictionary[title]()
```

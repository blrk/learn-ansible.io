# learn-ansible

YAML 
   <p> it is easier to read and write </p>

YAML Basics
   <p> --- --> shows the begining of YAML anything above that line shout not be parsed as YA
    every item in the list is a list of key/value pairs 
    commonly known as hash or a dictionary.
    we should learn how to write list and dictionaries 
    important 
        need to be careful about the white space. it matters!!! </p>
example 1

---
# list of car manufacturers --> this is a comment starts with "#" 
cars
  - Maruthi
  - Honda
  - Audi

example 2 

---
# type of car model produced by each manufacturers 
- ciaz
   colour: red
   price: 10L
   engine: hybrid

First apache playbook

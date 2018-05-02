# learn-ansible

YAML 
   <p> it is easier to read and write </p>

YAML Basics
   <p> 
        <ul> 
            <li> --- --> shows the begining of YAML anything above that line shout not be parsed as YAML </li>
            <li> every item in the list is a list of key/value pairs, commonly known as hash or a dictionary </li>
            <li>we should learn how to write list and dictionaries </li>
            <li>need to be careful about the white space. it matters!!! </li>
        <ul>
    </p>
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

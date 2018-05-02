<!DOCTYPE html>
<html>
<head>
    <style>
        pre {
            display: block;
            font-family: campriya;
            white-space: pre;
            margin: 1em 0;
            color: rgb(250,250,250);
            background-color: gray;
        } 
    </style>
<body>
#learn-ansible
YAML 
   <ul> <li> it is easier to read and write </li></ul>
YAML Basics
   <p> 
        <ul> 
            <li> --- shows the begining of YAML anything above that line shout not be parsed as YAML </li>
            <li> every item in the list is a list of key/value pairs, commonly known as hash or a dictionary </li>
            <li>we should learn how to write list and dictionaries </li>
            <li>need to be careful about the white space. it matters!!! </li>
        <ul>
    </p>
<p> <b> example 1 </b> </p>

<div>
    <pre>
        --- 
        # list of car manufacturers --> this is a comment starts with "#" 
        cars
          - Maruthi
          - Honda
          - Audi
    </pre>
</div>
<b>example 2 </b>
<div>
    <pre>
        ---
        # type of car model produced by each manufacturers 
        - ciaz
           colour: red
           price: 10L
           engine: hybrid
    </pre>
</div>
<div>
    <a href="apache.yml">First apache playbook</a>
</div>
</body>
</html>

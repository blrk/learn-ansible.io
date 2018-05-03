    
<h2>learn-ansible</h2>
<br/>
<b>YAML</b> 
   <ul> <li> it is easier to read and write </li></ul>
<b>YAML Basics</b>
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
        cars
          - Marthi
            Model: Ciaz
            colour: red
            price: 10L
            engine: hybrid
    </pre>
</div
<div>
    <h2> Install Ansibe in Centos 7 </h2>
    <pre>
        yum install -y epel-release
        yum install -y ansible
    </pre>
    <h2> Check the version of the Ansible </h2>
    <pre>
        ansible --version
    </pre>
    <h2> Create and add host key to enable password less login</h2>
    <pre>
        ssh-keygen -t rsa -b 4096
        ssh-copy-id root@192.168.100.160 # replace the ip with your own ip
    </pre>
    <h2> Configure the host file in /etc/ansible/hosts </h2>
    <pre>
        [webservers] # webserver group 
        webserver1 ansible_ssh_host=192.168.100.160
        webserver2 ansible_ssh_host=192.168.100.161
        #webserver3.example.com 
        192.168.100.162        
        #create your ungrouped hosts like this
        ftpserver1.example.com
        192.168.100.163
    </pre>
    <h2> Check the connectivity with the hosts </h2>
    <pre>
        # it will ping all the nodes
        # Note it is not the network ping
        ansible -m ping all 
        # ping a single node
        ansible -m ping webserver1
        # output
        webserver1 | SUCCESS => {
            "changed": false, 
            "ping": "pong"
        }
    </pre>
</div>
<div>
    <a href="apache.yml">First apache playbook</a>
</div>


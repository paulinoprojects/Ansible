# Ansible Fundamentals & Archtechture
 - <b>Control Node</b> - A system which Ansible is installed. You run Ansible commands: ansible or ansible-inventory on a control node.
 - <b>Managed Node</b> - A remote system, host, that ansible controls.
 - <b>Inventory</b> - A list of managed nodes that are logically organized. You create an inventory on the control node to describe host deployments to ansible.
   - Inventories organizes managed nodes in centralized files that contains system information and network locations.
   - <b>Inventory Files</b> - Defines host and groups of hosts, which commands, modules, and task in a playbook.
     - Default location for inventory is a file called <b><i> /etc/ansible/hosts</b></i>
     - Characeristics of <b>YAML (.yaml)(.yml)</b>
     - Keys: Values, is how YAML is written
     - Data types for key (attribute): value
       - Strings
       - Integers
       - Boolean - true or false
       - List
       - Does not rely on brackets and quotations like JSON or XML, instead <b><i>spacing and indentation</b></i>.

![AnsibleBasic](https://user-images.githubusercontent.com/111991325/202610504-9af669fc-b6bc-417c-906e-03a0176b47ce.png)

# Components o


 
<b>Playbooks</b> - A single YAML file,
 - <b>Playbook</b>: the highest level, just a list of plays
   - <b>Play</b>: Ordered set of tasks that ties tasks to host lists
    - <b>Tasks</b>: definition of a call to a module
    - Besides tasks, a play may have pre-tasks, post-tasks and handlers, which are all task-like, and roles.
    - <b>Modules</b> are discrete units of code that can be used from the command line or in a playbook task.
 

- <b>Plays</b></b> - Defines a set of activities (tasks)
- <b>Task</b> - An action to be performed on the host(s)
  - Run a script or command
  - Restart/shutdown
  - Install a package
  - Commands
 
- Hosts: must be defined in the inventory file
- Commands: referred to as modules, and categorized based on functionality
   - System
   - Commands
   - Files
   - Database
   - Cloud
   - Windows


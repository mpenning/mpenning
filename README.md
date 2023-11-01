
<!--
**mpenning/mpenning** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
Hello 👋, I'm [Mike Pennington][1] a Network Engineer from Austin, TX.

- 💬 These are some things about:
  - My Projects
    - [CiscoConfParse][4] 
  - Misc Tools
    - [Taskwarrior][2] (also see [Usage examples][3])
```
##############################################################################
## Quick tutorial
##############################################################################
git clone git@github.com/GothenburgBitFactory/taskwarrior
cd taskwarrior
cmake -DCMAKE_BUILD_TYPE=release .
make
# Assume ~/bin is in your path... put it where you like 
cp src/task ~/bin/
# Add a new task, due in four hours
task add Build a new foo project:this status:pending due:+4h
# Make task /foo/ searches case-insensitive...
echo 'search.case.sensitive=no' >> ~/.taskrc
# Add a new task that depends on the first one, due at end of month
task add Build a new bar depends:1 project:this status:pending due:eom
# List the tasks (default in ~/.task/pending.data)
task
# Detail about task number 1
task 1
# Modify the project for task 1, and make it recur daily
task modify 1 project:that recur:daily
# Export tasks as json
task export
# Delete task number 1
task rm 1
```
    
[1]: http://pennington.net
[2]: https://github.com/GothenburgBitFactory/taskwarrior
[3]: https://taskwarrior.org/docs/examples/
[4]: https://github.com/mpenning/ciscoconfparse/

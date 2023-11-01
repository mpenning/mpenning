[mpenning / mpenning / README.md](https://github.com/mpenning/mpenning/blob/main/README.md "A place for my github profile")

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

- Network
  - [Cisco Systems][1]
- Tools
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
cp src/task ~/bin/task
# Add a new task due at the end of the month
task add Build a new foo project:this status:pending due:eom
# Add a new task that depends on the first one
task add Build a new bar depends:1 project:this status:pending due:eom
# List the tasks (default in ~/.task/pending.data)
task
# Detail about task number 1
task 1
# Export tasks as json
task export
# Delete task number 1
task rm 1
```
    

[1]: https://cisco.com/
[2]: https://github.com/GothenburgBitFactory/taskwarrior
[3]: https://taskwarrior.org/docs/examples/

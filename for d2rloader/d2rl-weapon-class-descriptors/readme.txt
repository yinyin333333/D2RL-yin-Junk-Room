plugins
d2rloader\plugins\d2rl-weapon-class-descriptors.dll
d2rloader\plugins\d2rl-weapon-class-descriptors.mpq

Let me give you an example.

First, split `mace` into `hammer`, `scepter`, and `club`. Then, in `itemtypes`, copy the `Sword` entry, change its code to `test`, and assign `test` to the Crystal Sword. In the example files, `Swordtest` uses the `test` code, and Crystal Sword has its type set to `test`.  

Next, go to:

`d2rloader\plugins\d2rl-weapon-class-descriptors.mpq\data\global\excel\d2rloader\weapon-class-descriptors\descriptors.txt`

Add the code you want to modify—or a new code you've created—and specify the corresponding string key for it.

Then, in:

`data\local\lng\strings\item-modifiers.json`

add the appropriate entry for the string key you specified in `descriptors.txt`, and customize the text however you want.

That's all.
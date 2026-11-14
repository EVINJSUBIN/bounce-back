# Bounce Back

The real Hack Club Haven project. `HCBgroup/bbGame` was practice. Do not build there anymore.

Godot **4.7** for everyone. Open this folder's `project.godot`.

First scenes we are locking in: **house** and **school**. The school hallway should loop. The house is one morning room. Title, roof, exam bar, and phone come after those two scenes run.

## Git setup

One repo. One branch: `main`. No feature branches today. Two people editing branches will spend the hour merging.

Both of you:

```bash
git clone https://github.com/HCBgroup/bounce-back.git
```

Before you edit, and again before you commit:

```bash
git pull
```

When a scene runs:

```bash
git add scenes/house.tscn scripts/house.gd
git commit -m "House: player can walk to the door"
git push
```

The other person then runs `git pull` and presses F5.

If Git says you are behind, pull before you push. If it talks about a conflict, stop and look at the file together. Do not use `--force`.

Commit the scene, the script, and the `.import` files Godot makes. Do not commit the `.godot/` folder. It is already ignored.

## Who edits what

Do not open the other person's scene while they have it unsaved.

| Files | Who |
| --- | --- |
| `scenes/house.tscn`, `scripts/house.gd` | one of you |
| `scenes/school.tscn`, `scenes/chunk.tscn`, `scripts/school.gd` | the other |
| `scenes/player.tscn`, `scripts/player.gd`, `project.godot` | whoever needs them, one at a time, then push immediately |

Say in the commit message which scene you touched.

## Playtest check

- House: he can walk and he cannot leave through the walls.
- School: hold right, the hallway does not end. Hold left, same thing.

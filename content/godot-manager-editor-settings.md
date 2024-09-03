+++
title = "Importing Editor Settings in a new version of Godot with Godot Manager"
date = 2024-09-03
+++

I use [Godot Manager](https://github.com/eumario/godot-manager) to manage which versions of Godot are installed on my system, it's a very useful tool when you have multiple projects going on at the same time using different versions of Godot.

I've recently updated to Godot 4.3, but my editor settings were not ported over. There is an option to link settings in Godot Manager, but for whatever reason it seems not to be working properly on my machine. Thankfully, porting settings manually is very easy.

All there is to know is that Godot Manager installs versions of Godot in [self-contained mode](https://docs.godotengine.org/en/stable/tutorials/io/data_paths.html#self-contained-mode), which stores all settings in the same folder where the binary for the editor is found.

Just hop over to wherever Godot Manager stores Godot versions on your machine (```%APPDATA%/Godot-Manager/versions/``` on Windows), and you can copy and paste the relevant editor_data folder to the version you just installed.

Not a very ambitious first blog entry, but hopefully that saved you a few minutes of googling.
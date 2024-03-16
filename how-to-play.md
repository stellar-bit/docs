# How To Play

## Understand what the game is

Stellar Bit provides a place where people can create their own custom servers for others to join them.

Players write or use other peoples scripts to empower them in controlling the game.

### Game Object

Some kind of object in space represented by physical properties such as position, mass, velocity, etc...

Consists of materials.

### Player

Can directly own game objects.

Has materials which he can use for example for building.

### Projectile - Game Object

Uncontrollable and usually spawned by player.

### Spacecrafts - Game Object

It is a collection of components where each component provides a functionality to the whole. This way players can build their spacecraft from these components based on intended purpose.

Components are of three types:
- blocks 
    - main building unit
    - vary in weight, toughness
- weapons
    - spawn projectiles
    - for mining 
    - for attacking
    - vary in projectiles
- engines 
    - for changing velocity of the spacecraft
    - capacity limited with 'fuel'

### Star Bases - Game Object

This is where spacecrafts are being built and deployed. 

### Asteroids - Game Object

Can be damaged for materials.

## Running a client

The official Stellar Bit client along with installation instructions can be found at https://github.com/stellar-bit/client-basic.

You can run the client offline or connect to a server through the `Network connection` window.

If you want to connect to public servers and have an official Stellar Bit account, connect to the central hub through the `Central Hub` window as well, to see all officially hosted public servers.

To control the game you need to load a `computer` through the `Controller` window. To obtain a `computer` follow the next section.

## Making a computer

Computer is a file created by the user, that contains a computation which executes game commands for the user, based on some logic which can include user interaction.

Programming language for computers that is currently supported is `Rust`, but technically anything will work since `Rust` can interface with other langauges as well.

The main user interaction which is currently supported is `egui` it provides a simple framework to create UI and get the input from user.

It is recommended to start with the `computer-template` repo which can be found here: https://github.com/stellar-bit/computer-template.

Download the repository and open the folder in your code editor.

Now you can edit the logic of the computer but first let's compile the downloaded template and open it in our client.

1. Compilation: in the directory of the computer, execute a bash file called `build.sh`, and everything should build smoothly
2. Open file in client: the built computer should be located in the subfolder `dist/`, open it from the client in the `Controller` window
3. New `egui` windows in the client should appear, test whether it works as expected

Now you can make modifications to the `computer-template` and follow the same steps to recompile and open it again.




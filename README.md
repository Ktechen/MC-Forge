## MC-Forge

### How to install minecraft mod server?

#### Download links [requird]
[Forge](http://files.minecraftforge.net/maven/net/minecraftforge/forge/index_1.12.2.html)

#### Hexxit mod 
[Hexxit](https://media.forgecdn.net/files/2972/393/Hexxit+Updated+Server+Pack.zip)
[CTM](https://media.forgecdn.net/files/2915/363/CTM-MC1.12.2-1.0.2.31.jar)

### Client Part

1. Install client part of forge

![alt text](https://github.com/Ktechen/MC-Forge/blob/master/pic/Client.PNG)

2. Start Minecraft and edit JVM-Argumente

```JVM-Argumente
-Xmx2G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
```
3. Change -Xmx2G to -Xmx16G (G = Gibibyte)

4. Add mods 

```%appdata%
Open: %appdata% and then open .minecraft/mods
```

### Server Part

1. Install Linux distributionen like Ubuntu, Debian ...
2. Create new user | ``` adduser "Name" ```

![alt text](https://github.com/Ktechen/MC-Forge/blob/master/pic/adduser.PNG)

3. Download server
4. Open folder : ``` cd home/test123 ``` 
5. Change profil: ``` su test123 ``` 
6. Download Server: ``` wget https://files.minecraftforge.net/maven/net/minecraftforge/forge/1.12.2-14.23.5.2854/forge-1.12.2-14.23.5.2854-installer.jar ``` 
####(Tipp: For Copy and Paste use SHIFT + INSERT)

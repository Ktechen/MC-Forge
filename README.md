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
2. Create new user: ``` adduser "Name" ```

![alt text](https://github.com/Ktechen/MC-Forge/blob/master/pic/adduser.PNG)

3. Open folder : ``` cd home/test123 ``` 
4. Change profil: ``` su test123 ``` 
5. Download Server: ``` wget https://files.minecraftforge.net/maven/net/minecraftforge/forge/1.12.2-14.23.5.2854/forge-1.12.2-14.23.5.2854-installer.jar ``` 
#### (Tipp: For Copy and Paste use SHIFT + INSERT)
6. Install Server: ``` java -jar forge-1.12.2-14.23.5.2854-installer.jar --installServer ```
7. First start: ``` java -jar forge-1.12.2-14.23.5.2854.jar ```
8. Agree EULA: ``` vim eula.txt  ```
#### (Tipp: Press I to Insert, control+c to cancel and :wq to save current file) 
9. Create file: ``` vim launch.sh ``` Copy and Paste: ``` #!/bin/sh java -Xmx16G -Xms2G -jar forge-1.12.2-14.23.5.2854.jar -nogui ```
10. Create executable file: ``` chmod u+x launch.sh ```
11. Open Screen or create a service: ``` screen ``` and then: ./launch.sh (Service https://wiki.ubuntuusers.de/Howto/systemd_Service_Unit_Beispiel/)

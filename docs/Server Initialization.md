---
layout: default
title: Server Initialization
nav_order: 2
---

# Server Initialization
{: .no_toc }

These are the steps you will take to start running your Minecraft server.

The first task we need to do to set up and host a Minecraft: Java Edition Server is to download the Minecraft Server `.jar` file, also called a Java ARchive file, install it, and then change its configuration settings. This task will require you to use of the Command Prompt app and run some command lines. But do not worry, we will guide you through every step of the process!

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Getting Started

1. Before we download the `.jar` file, we need to create a folder to keep all of the server files in. Create the folder on your desktop and name it “Minecraft Server”.

2. Go to [www.minecraft.net/en-us/download/server](https://www.minecraft.net/en-us/download/server) and download the `minecraft_server.1.XX.X.jar` file and save the file in the “Minecraft Server” folder we created.

    ![Minecraft Task](../assets/images/server/Task1.01.PNG)

3. In order to run the commands in the Command Prompt, we need to know the location, or filepath, of the `.jar` file we downloaded. We can determine the file path by opening the folder and clicking on the address bar near the top.  In this example, the file path is: `C:\Users\lbeiq\Desktop\Minecraft Server`.

    ![Minecraft Task](../assets/images/server/Task1.03.png)

## Starting the Server

1. To proceed with the next steps. we need to open up the Command Prompt application. On your desktop, go to the bottom left search bar and type in “Command Prompt”.

    ![Minecraft Task](../assets/images/server/Task1.02.png)
   
2. In the command prompt, type the command: `cd` followed by a space and then the file path to the location of the `.jar` file. Hit enter to run the command.  In this example, the command is: `cd C:\Users\lbeiq\Desktop\Minecraft Server`.

3. Once you are in the correct directory in the command prompt, type the command: `Java -jar` followed by a space and the name of your `.jar` file. Hit enter to run the command. In this example, the command is: `Java -jar server.jar`.

    ![Minecraft Task](../assets/images/server/Task1.04.png)
    
## Changing the Configurations

1. In the Minecraft Server folder, open the `eula.txt` file by double-clicking it. Inside the file, change the line `eula=false` and replace it with the line `eula=true`. You might notice a star in the file header in the top left. This indicates that there are unsaved changes. Make sure to save your changes and then close the file.

    ![Minecraft Task](../assets/images/server/Task1.05.PNG)

    ![Minecraft Task](../assets/images/server/Task1.06.png)

    ![Minecraft Task](../assets/images/server/Task1.07.png)

2. Locate the server file with the file type: `properties source file`, and then right-click it, select Open with, and then Choose another app. Next, click on more apps, and scroll down until you find Notepad. Select Notepad and the file should open up with all of the Minecraft server properties.

    ![Minecraft Task](../assets/images/server/Task1.08.png)

    ![Minecraft Task](../assets/images/server/Task1.09.png)

    ![Minecraft Task](../assets/images/server/Task1.11.png)

3. Look for the `query.port` line and write down the port number. This will be important when we forward the ports in [Port Forwarding](https://lbeique.github.io/How-To-Setup-a-Minecraft-Server/docs/PortForward/), to allow other users to join the server.

    ![Minecraft Task](../assets/images/server/Task1.13.png)
    
    You probably noticed there are a lot more settings in this file that can enhance your play experience, and we strongly recommend you take a [detailed](https://minecraft.fandom.com/wiki/Server.properties) look through them at a later time.
    
## Running the Server

1. Now that we have the port number recorded, we return to the command prompt app. To run the server, simply repeat the steps from [Starting the Server](https://lbeique.github.io/How-To-Setup-a-Minecraft-Server/docs/Server%20Initialization/#starting-the-server). If you get a Windows Security Alert, simply Allow access to Private networks, such as my home or work network.

    ![Minecraft Task](../assets/images/server/Task1.22.png)

2. And thats it! Your server should now be running! If you want to close your server, simply close the Minecraft server app and the server will turn off.

    ![Minecraft Task](../assets/images/server/Task1.23.png)

## Conclusion
{: .no_toc }

Great job! Next we will [forward the server port](https://lbeique.github.io/How-To-Setup-a-Minecraft-Server/docs/PortForward/) so that we can invite other users to the Minecraft Server!

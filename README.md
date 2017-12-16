First install flatpak for your distro. 


**To build the flatpak:**  
Install lutris for your distro: https://lutris.net/  

In lutris menus: Lutris>Manage Runners>Wine>Manage Versions  
check the box next to staging-2.21 i386 and wait for it to install.  

Then:

git clone http://www.github.com/gloriouseggroll/flatpak-leagueoflegends.git  
cd flatpak-leagueoflegends  
 ./flatpak-make leagueoflegends leagueoflegends LeagueClient.exe  
cd target/[Flatpak-Riot\ Games]leagueoflegends/  

**To install the flatpak:**  
chmod +x *.sh  
./install  
./run  

if you need to remove:  
./uninstall  

wine prefix is located in ~/.local/share/flatpak-riotgames/leagueoflegends  
see leagueoflegends.md located inside the wine prefix for useful wine commands.  

You can run the game with command:  
flatpak run org.RiotGames.leagueoflegends  

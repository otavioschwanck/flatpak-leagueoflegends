First install flatpak for your distro. 


**To build the flatpak:**  

git clone http://www.github.com/gloriouseggroll/flatpak-leagueoflegends.git  
cd flatpak-leagueoflegends  
 ./flatpak-make leagueoflegends leagueoflegends LeagueClient.exe i386

**To install the flatpak:**  
flatpak --user remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo  
flatpak --user install -y --app --bundle "leagueoflegends.flatpak"  
flatpak --user install flathub org.freedesktop.Platform.GL.default/i386/1.6  
flatpak run org.RiotGames.leagueoflegends  

If you need to remove:  
(If you need to make a backup of your League install, copy the Riot Games folder from ~/.local/share/flatpak-riotgames/leagueoflegends/drive_c/)  
flatpak --user uninstall org.RiotGames.leagueoflegends  
sudo rm -R ~/.local/share/flatpak-riotgames  

wine prefix is located in ~/.local/share/flatpak-riotgames/leagueoflegends  
see leagueoflegends.md located inside the wine prefix for useful wine commands.  

You can run the game with command:  
flatpak run org.RiotGames.leagueoflegends  

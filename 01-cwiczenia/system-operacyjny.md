## System operacyjny w środowisku sieciowym

### Zadania


1. Z wykorzystaniem maszyny wirtualnej, zainstaluj SO oraz wypisz parametry konfiguracji IP tj:
   * Adres
   * Maska
   * Adres bramy
   * DNS 1
   * DNS 2
    
    Powyższe parametry uzyskaj na wszystkich z wymienionych systemów

   * [Linux Alpine](https://alpinelinux.org/)
   * [Linux Debian](https://www.debian.org/)
   * [Linux CentOS](https://www.centos.org/)
   * Windows 

2. Sprawdź oraz przygotuj charakterystykę dla przykładowego urządzenia w Twojej sieci domowej
   * Adres
   * Maska
   * Adres bramy
   * DNS 1
   * DNS 2
  
    Przygotuj dokumentację graficzną Twojej sieci domowej, uwzględnij adresy i urządzenia

3. Zarejestruj konto w CISCO Academy celem pobrania Packet tracer 
   https://www.netacad.com/courses/packet-tracer


### Charakterystyka systemu operacyjnego

| Charakterystyka           | wartość               | komentarzu                |
| -------------             |:-------------:        | -----:                    |
| nazwa                     | linux                 | centos 7                  |
| cfg interfejsów           | centos 7 | /etc/sysconfig/network-scripts         |
| program (parametry sieci) | niewiem               |                           |
| ....                      | .....                 |                           |
| nazwa                     | Alpine Linux          |                           |
| Konfiguracja ip           | ``$ ip all ``         | show all eth interfaces   | 
| Tablica routingu          | ``$ ip route show ``  | what is gateway?!         | 
| check nameservers (DNS)   | ``$ cat /etc/resolv.conf ``  | which DNS were set | 

### Konfiguracja połączenia sieciowego

| Parametr | wartość           | komentarzu |
| ------------- |:-------------:| -----:|
| Adres IP      | 10.0.2.15/24        | ip addr / ip addr show {eth0}       |
| Maska podsieci| 255.255.255.0       |  ip addr / ip addr show {eth0}      |
| Brama         | 10.0.2.2            |  ip route / netstat -r {default / *} |
| DNS 1         | 8.8.8.8             |  cat /etc/resolv.conf    |
| DNS 2         | 1.1.1.1             |    |

### Schemat sieci

aby załączyć obrazek 

```markdown
![alt schemat](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)![alt schemat](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png)

![alt schemat](images/my-network-schema.png)
```

![my network](network.png)

### Wirtualizacja typy sieci

Przetestuj parametry sieci dla różnych typów wspieranych przez Twoje oprogramowanie. każdą konfigurację opatrz komentarzem co do funkcjonalności. 
* połączenie z internetem Tak / Nie
* połączenie z innymi wirtualnymi maszynami Tak / Nie
* połączenie z komputerem Hostem Tak / Nie
* połączenie z innymi urządzeniami w sieci Hosta Tak / Nie



-------------------------
| Program | Typ | komentarz(opcionalny) |
| ------------- |:-------------:| -----:|
|Virtualbox|bridge||
|Virtualbox|hostonly||
|Virtualbox|nat||


### Ustawienia dla innego oprogramowania
#### Docker
https://docs.docker.com/network/#network-drivers

#### VMware
https://docs.vmware.com/en/VMware-Workstation-Player-for-Windows/16.0/com.vmware.player.win.using.doc/GUID-C82DCB68-2EFA-460A-A765-37225883337D.html

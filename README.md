# Образы Docker для панели Pterodactyl

Образы основаны на Java Azul Zulu. Версии старше 8 (включительно) содержат поддержку webp для корректной работы DynMap.

## Зачем это всё?

Плагины, используемые на моих серверах плохо поддерживают дефолтную Open JRE. На просторах нашёл образы [Alex](https://github.com/Software-Noob). 
Там была требуемая Azul Zulu, но не было 7 версии - решил не беспокоить автора и сделать самостоятельно. Позже выяснилось, что в остальных образах отсутствует компонент webp, 
из-за чего карта в Dynmap сохраняет элементы в формате jpg, что тоже не очень. Так появились остальные пакеты.


Дополнительные образы для панели можете найти в репозиториях: [Alex](https://github.com/Software-Noob/pterodactyl-images), [Parkervcp](https://github.com/parkervcp/images), [Matthewpi](https://github.com/matthewpi/images) и [Yolks](https://github.com/pterodactyl/yolks).

## Как добавить образ

Перейдите в `Admin Panel -> Nests -> Select your egg`. Добавьте требуемые адреса образов Docker из списка ниже:

Java 17 Zulu (webp)|ghcr.io/mfc166/pterodactyl-images:java_17_zulu  
Java 11 Zulu (webp)|ghcr.io/mfc166/pterodactyl-images:java_11_zulu  
Java 8 Zulu (webp)|ghcr.io/mfc166/pterodactyl-images:java_8_zulu  
Java 7 Zulu|ghcr.io/mfc166/pterodactyl-images:java_7_zulu

![image](https://user-images.githubusercontent.com/10975908/120903180-56719d80-c64d-11eb-8666-02de8ea80701.png)

### Java Azul Zulu [AMD64]

- [Java 7 Zulu](https://github.com/mfc166/pterodactyl-images/tree/main/java-zulu/7)
  - `ghcr.io/mfc166/pterodactyl-images:java_7_zulu`
- [Java 8 Zulu + WebP](https://github.com/mfc166/pterodactyl-images/tree/main/java-zulu/8)
  - `ghcr.io/mfc166/pterodactyl-images:java_8_zulu`
- [Java 11 Zulu + WebP](https://github.com/mfc166/pterodactyl-images/tree/main/java-zulu/11)
  - `ghcr.io/mfc166/pterodactyl-images:java_11_zulu`
- [Java 17 Zulu + WebP](https://github.com/mfc166/pterodactyl-images/tree/main/java-zulu/17)
  - `ghcr.io/mfc166/pterodactyl-images:java_17_zulu`

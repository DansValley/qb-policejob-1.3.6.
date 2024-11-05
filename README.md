qb-policejob
QB-Core Framework için Polis İşleri :police_officer:

Bu, resmi qb-policejob'un ek özelliklerle düzenlenmiş bir versiyonudur.

Güncellemeler
v1.3.0

Kelepçe, zip bağ, kırık kelepçeler, kelepçe anahtarları, bolt kesici ve flush kesici eklendi

Oyuncuları kelepçeleyebilir ve kelepçe anahtarlarıyla çözülebilirsiniz

Sadece kelepçelerin olduğu taraftan (ön / arka) çözülebilirsiniz (zip bağlar için de aynı)

Oyuncuları zip bağlayabilir ve flush kesici ile kesebilirsiniz

Yasal olmayanlar, kelepçeleri kesmek için bolt kesici kullanabilir ve kırık kelepçeler alır


v1.3.1

Kelepçe kullanıldığında, kelepçe anahtarı alırsınız ve kelepçeler kaldırılır

Anahtar kullandığınızda, anahtar kaldırılır ve tekrar kelepçeleri alırsınız

Araç giydirme menüsü eklendi

Polis araçları için fiyatlar eklendi


v1.3.2 :

Zip bağlar için yeni nesne eklendi

Önceden kelepçelenmiş oyuncuların soygun yapma sorunu düzeltildi

Yapılandırılabilir kelepçe türleri eklendi, burada hangi tür kelepçe ile oyuncunun hareket edip edemeyeceğini seçebilirsiniz



v1.3.3

Parmak izi UI'sı değiştirildi

Delil araştırma seçeneği eklendi. Polis, dolu delil çantalarını laboratuvarında araştırabilir ve delil hakkında daha fazla bilgi görebilir

Polis için depo ve çekme sistemi değiştirildi. Araç üzerine hedef kullanarak depo/çekim ücreti alabilirsiniz

Vatandaşlar polis çekme alanına erişebilir ve kendi araçlarını görebilir. Ücreti ödediklerinde kendi araçlarını alabilirler

Kurtulma seçeneği eklendi. Bunu yapılandırmada etkinleştirirseniz, kelepçelenmiş oyuncu bir mini oyun görecektir ve başarılı olursa kaçabilir.

Depo/çekim için negatif miktar problemleri düzeltildi

Eksik ifadelerle ilgili uyarı düzeltildi

Ölü veya son aşamada olan oyuncular için animasyon düzeltmesi



v1.3.4

Genel delil deposunun açılmama problemi düzeltildi

Kurtulma sistemi için ps-ui seçeneği eklendi

Başarıyla kelepçelenen veya vatandaşın kurtulduğunda, polise bildirim gönderilecek

qb-target / qtarget / ox_target desteği eklendi

Parmak izi görüntüsünün yanlış kişiyi göstermesi düzeltildi

Ateş ederken mermi düşürme olasılığı artırıldı

LEO iseniz, ateş ederken mermi düşüremezsiniz

Blip ağ olayı optimize edildi

v1.3.5

Laboratuvar delil menüsünün kan veya parmak izi göstermemesi düzeltildi (teşekkürler @ F7)

Birini eskort ederken polislerin koşma / zıplama durumu devre dışı bırakıldı


v1.3.6

Script başlatıldığında hedeften kaynaklanan hata düzeltildi

Blip sistemi optimize edildi

Her ayrı LEO iş için renk seçenekleri eklendi (bcso = turuncu, polis = mavi, sasp = yeşil vb.)

Blip'lerin etkinleştirilmesi/devre dışı bırakılması için leo-gps nesnesi eklendi (resimler klasörü içinde)

GPS nesnenizi kaybettiğinizde veya düşürdüğünüzde, blip'iniz silinecek (birisi sizi soygun yapar ve GPS'inizi alırsa)

Araç türüne göre farklı blip sprite'ları (helikopter, bot, uçak, motosiklet, acil durum araçları ve diğer tüm araçlar için)
Mevcut

Görevde / görev dışı, kıyafet, araç, depo vb. gibi klasik gereksinimler

Vatandaş kimlik tabanlı silah deposu (Beyaz listeye alınmış)

Parmak izi testi

Delil deposu (depo)

Beyaz listeye alınmış araçlar

Harita üzerindeki hız radarları

Stormram

Oyuncu aracını çekme (kalıcı / belirli bir ücret karşılığında)

Entegre hapishane sistemi

Mermi kovanları

GSR


Kan damlası

Delil çantası ve para çantası

Polis radarı

Kelepçe bir nesne olarak (Komutlar bölümünü kontrol edin. Komutlar bölümünde kullanılabilir.)

Acil durum hizmetleri haritada birbirlerini görebilir

Kurulum

Resimler klasöründeki resimleri envanter resimleri klasörünüze kopyalayın

Aşağıdaki öğeleri qb-core\shared\items.lua dosyanıza ekleyin



# qb-policejob
Police Job for QB-Core Framework :police_officer:

This is an edited version of the official qb-policejob with added features.


## Updates

v1.3.0
- Added cuff, ziptie, broken handcuffs, cuffkeys, bolt cutter and flush cutter
- You can cuff players with handcuffs and uncuff them with cuffkeys
- You can only uncuff them from the side (front / back) where the cuffs are (same for zipties)
- You can ziptie players and cut it with flush cutter
- Illegals can use bolt cutter to cut the cuffs and will get broken cuffs

v1.3.1
- When used cuff, you'll get cuff key and cuffs will be removed
- When you use keys, it will be removed and give you cuffs again
- Added vehicle livery menu
- Added prices for police vehicles

v1.3.2 :

- Added new prop item for zipties
- Fixed the rob player when cuffed from front
- Added configurable cufftypes into config where you can choose from wether the player can move with that kind handcuffs or not

v1.3.3
- Fingerprint UI has been changed
- Added evidence research option. Police can research filled evidence bags in lab and will see more info about the evidence
- Changed depot and impound system for police. Able to use target on vehicle and charging for depot / impound
- Citizens can access police impound and will see their own cars. When they pay the charge they can get their own vehicle
- Added breakout option. When you enable this in config, the cuffed player will see a minigame and when they success they can escape.
- Fixed the problem with negative amounts for depot / impound
- Fixed warning with missing phrases
- Animation fix for dead or in last stand players

v1.3.4
- Fixed general evidence stash not opening problem
- Added ps-ui option for breakout system
- Officier will get notification when successfully cuffed or citizen broke out
- Added support for qb-target / qtarget / ox_target
- Fixed fingerprint image showing wrong person
- Added more possibility to drop bullet when shooting
- If you are LEO then you can't drop bullets when shooting
- Optimize blips network event

v1.3.5
- Fixed lab evidence menu not showing with blood or fingerprint (thnx @ F7)
- Disabled police running / jumping when escorting someone

v1.3.6

- Fixed the error from target when starting the script up
- Optimized the blip system
- Added color options for each seperate LEO job (bcso = orange, police = blue, sasp = green etc.)
- Added leo-gps item for activating / deactivating the blips (inside images folder)
- When you loose or drop your gps item, your blip will be deleted (when someone robs you and gets your gps)
- Different blip sprites depending on vehicle type (heli, boats, plane, motorbike, emergency vehicles and for all other vehicles)

### Existing
- Classical requirements like on duty/off duty, clothing, vehicle, stash etc.
- Citizen ID based armory (Whitelisted)
- Fingerprint test
- Evidence locker (stash)
- Whitelisted vehicles
- Speed radars across the map
- Stormram
- Impounding player vehicle (permanent / for an amount of money)
- Integrated jail system
- Bullet casings
- GSR
- Blood drop
- Evidence bag & Money bag
- Police radar
- Handcuff as an item (Can used via command too. Check Commands section.)
- Emergency services can see each other on map

## Installation

- Copy images from images folder to your inventory images folder

- Add the below items to your qb-core\shared\items.lua

```
	['broken_handcuffs'] 			 = {['name'] = 'broken_handcuffs', 			    ['label'] = 'Broken Handcuffs', 		['weight'] = 100, 		['type'] = 'item', 		['image'] = 'broken_handcuffs.png', 	['unique'] = false, 	['useable'] = false, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'It\'s broken, maybe you can repair it?'},
	['cuffkeys'] 				 	 = {['name'] = 'cuffkeys', 			    		['label'] = 'Cuff Keys', 				['weight'] = 75, 		['type'] = 'item', 		['image'] = 'cuffkeys.png', 			['unique'] = false, 	['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Set them free !'},
	['ziptie'] 				 	 	 = {['name'] = 'ziptie', 			    		['label'] = 'ZipTie', 					['weight'] = 50, 		['type'] = 'item', 		['image'] = 'ziptie.png', 				['unique'] = false, 	['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Comes in handy when people misbehave. Maybe it can be used for something else?'},
	['flush_cutter'] 				 = {['name'] = 'flush_cutter', 			    	['label'] = 'Flush Cutter', 			['weight'] = 50, 		['type'] = 'item', 		['image'] = 'flush_cutter.png', 		['unique'] = false, 	['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Comes in handy when you want to cut zipties..'},
	['bolt_cutter'] 				 = {['name'] = 'bolt_cutter', 			    	['label'] = 'Bolt Cutter', 				['weight'] = 50, 		['type'] = 'item', 		['image'] = 'bolt_cutter.png', 			['unique'] = false, 	['useable'] = true, 	['shouldClose'] = true,	   ['combinable'] = nil,   ['description'] = 'Wanna cut some metal items ?'},
        ['leo-gps']                         = {['name'] = 'leo-gps',                           ['label'] = 'LEO GPS',                   ['weight'] = 2000,         ['type'] = 'item',         ['image'] = 'leo-gps.png',                 ['unique'] = true,          ['useable'] = true,      ['shouldClose'] = true,      ['combinable'] = nil,   ['description'] = 'Show your gps location to others'},


```

- Update the filled evidence bag in you qb-core/shared
````
    ['filled_evidence_bag']             = {['name'] = 'filled_evidence_bag',               ['label'] = 'Evidence Bag',              ['weight'] = 200,          ['type'] = 'item',         ['image'] = 'evidence.png',                ['unique'] = true,          ['useable'] = true,     ['shouldClose'] = true,     ['combinable'] = nil,   ['description'] = 'A filled evidence bag to see who committed the crime >:('},
````


- Update the filled evidence bag in your qb-inventory/html/js/app.js
```
else if (itemData.name == "filled_evidence_bag") {
    $(".item-info-title").html("<p>" + itemData.label + "</p>");
        if (itemData.info.type == "casing") {
            if (itemData.info.evidenceNote != null) {
                $(".item-info-description").html(
                    "<p><strong>Evidence material: </strong><span>" + itemData.info.label + "</span></p>" +
                    "<p><strong>Type number: </strong><span>" + itemData.info.ammotype + "</span></p>" +
                    "<p><strong>Caliber: </strong><span>" + itemData.info.ammolabel + "</span></p>" +
                    "<p><strong>Serial: </strong><span>" + itemData.info.serie + "</span></p>" +
                    "<p><strong>Crime scene: </strong><span>" + itemData.info.street + "</span></p>" +
                    "<br /><p><strong>Note Writer: </strong><span>" + itemData.info.noteWrite + "</span></p>" +
                    "<p><strong>Note: </strong><span>" + itemData.info.evidenceNote + "</span></p>"
                );
            } else {
                $(".item-info-description").html(
                    "<p><strong>Evidence material: </strong><span>" + itemData.info.label + "</span></p>" +
                    "<p><strong>Type number: </strong><span>" + itemData.info.ammotype + "</span></p>" +
                    "<p><strong>Caliber: </strong><span>" + itemData.info.ammolabel + "</span></p>" +
                    "<p><strong>Serial: </strong><span>" + itemData.info.serie + "</span></p>" +
                    "<p><strong>Crime scene: </strong><span>" + itemData.info.street + "</span></p>" +
                    "<br /><p>" + itemData.description +"</p>"
                );
            }
        } else if (itemData.info.type == "blood") {
            if (itemData.info.evidenceNote != null) {
                $(".item-info-description").html(
                    "<p><strong>Evidence material: </strong><span>" + itemData.info.label +"</span></p>" +
                    "<p><strong>Blood type: </strong><span>" + itemData.info.bloodtype +"</span></p>" +
                    "<p><strong>DNA Code: </strong><span>" + itemData.info.dnalabel +"</span></p>" +
                    "<p><strong>Crime scene: </strong><span>" + itemData.info.street +"</span></p>" +
                    "</br><p><strong>Note Writer: </strong><span>" + itemData.info.noteWrite + "</span></p>" +
                    "<p><strong>Note: </strong><span>" + itemData.info.evidenceNote + "</span></p>"
                );
            } else {
                $(".item-info-description").html(
                    "<p><strong>Evidence material: </strong><span>" + itemData.info.label +"</span></p>" +
                    "<p><strong>Blood type: </strong><span>" + itemData.info.bloodtype +"</span></p>" +
                    "<p><strong>DNA Code: </strong><span>" + itemData.info.dnalabel +"</span></p>" +
                    "<p><strong>Crime scene: </strong><span>" + itemData.info.street +"</span></p>" +
                    "<br /><p>" + itemData.description + "</p>"
                );
            }
        } else if (itemData.info.type == "fingerprint") {
            if (itemData.info.evidenceNote != null) {
                $(".item-info-description").html(
                    "<p><strong>Evidence material: </strong><span>" + itemData.info.label + "</span></p>" +
                    "<p><strong>Fingerprint: </strong><span>" + itemData.info.fingerprint + "</span></p>" +
                    "<p><strong>Crime Scene: </strong><span>" + itemData.info.street + "</span></p>" +
                    "</br><p><strong>Note Writer: </strong><span>" + itemData.info.noteWrite + "</span></p>" +
                    "<p><strong>Note: </strong><span>" + itemData.info.evidenceNote + "</span></p>"
                );
            } else {
                $(".item-info-description").html(
                    "<p><strong>Evidence material: </strong><span>" + itemData.info.label + "</span></p>" +
                    "<p><strong>Fingerprint: </strong><span>" + itemData.info.fingerprint + "</span></p>" +
                    "<p><strong>Crime Scene: </strong><span>" + itemData.info.street + "</span></p>" +
                    "<br /><p>" + itemData.description + "</p>"
                );
            }

        } else if (itemData.info.type == "dna") {
            if (itemData.info.evidenceNote != null) {
                $(".item-info-description").html(
                    "<p><strong>Evidence material: </strong><span>" + itemData.info.label + "</span></p>" +
                    "<p><strong>DNA Code: </strong><span>" + itemData.info.dnalabel + "</span></p>" +
                    "</br><p><strong>Note Writer: </strong><span>" + itemData.info.noteWrite + "</span></p>" +
                    "<p><strong>Note: </strong><span>" + itemData.info.evidenceNote + "</span></p>"
                );
            } else {
                $(".item-info-description").html(
                    "<p><strong>Evidence material: </strong><span>" + itemData.info.label + "</span></p>" +
                    "<p><strong>DNA Code: </strong><span>" + itemData.info.dnalabel + "</span></p>" +
                    "<br /><p>" + itemData.description + "</p>"
                );
            }
        }
    }
```

## Dependencies
- [qb-core](https://github.com/qbcore-framework/qb-core)
- [qb-management](https://github.com/qbcore-framework/qb-management) - For the boss/gang menu
- [qb-garages](https://github.com/qbcore-framework/qb-garages) - For the vehicle spawner
- [qb-clothing](https://github.com/qbcore-framework/qb-clothing) - For the locker room
- [qb-phone](https://github.com/qbcore-framework/qb-phone) - For the MEOS app and notifications etc.
- [qb-smallresources](https://github.com/qbcore-framework/qb-smallresources) - qb-log was added to qb-smallresources
- [qb-menu](https://github.com/qbcore-framework/qb-menu) - For the vehicle menus
- [qb-input](https://github.com/qbcore-framework/qb-input) - For accessing evidence stashes

### Commands
https://docs.qbcore.org/qbcore-documentation/qbcore-resources/qb-policejob#commands

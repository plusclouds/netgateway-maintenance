### PlusClouds.Automation.NetGateway
---

Bu modül PlusClouds'un kendi geliştirdiği basit Gateway'dir. Temel bir takım NFV 
ihtiyaçlarını gidermek adına geliştirilmiştir, bu özelliklerin üzerinde müşteri 
çeşitli özellikler istediği taktirde sanal Juniper veya sanal Cisco gateway'ler 
verilebilir.

Bu modül aşağıdaki özellikleri sağlamaktadır. Sağlamadığı söylenen özellikler
yol haritasında bulunduğu anlamına gelmektedir;

- Temel İşlevler
- - [x] NetGateway otomatik yaratılması
- - [ ] Reset to factory
- [ ] Ağ Yönetimi ()
- - [ ] Ağ'a bağlanma
- - [ ] Ağ trafiğini üzerinden akıtmak ve gateway görevi görmek
- [ ] VPN Yönetimi
- - [ ] VPN yaratma
- - [ ] VPN trafik izleme
- - [ ] PlusClouds IAM desteği
- [x] Proxy yönetimi
- - [x] Proxy kuralı yaratma
- - [ ] Proxy kuralı silme
- - [ ] Proxy kuralı izleme
- [ ] Load Balancer yönetimi
- - [ ] LB host yaratma
- - [ ] LB trafik dengesi denetimi yapma
- - [ ] LB trafik izleme
- [x] NAT yönetimi
- - [x] NAT kuralı yaratma
- - [ ] NAT kuralı silme
- [ ] Firewall Yönetimi
- - [ ] IPTables kuralları yönetimi

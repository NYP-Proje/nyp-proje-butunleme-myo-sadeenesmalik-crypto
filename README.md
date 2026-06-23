Elektrik Faturalama Sistemi (Electricity Billing System)

> Abone bilgilerini yöneten, elektrik tüketim endekslerine göre otomatik fatura hesaplayan ve fatura takibini kolaylaştıran modern bir faturalama otomasyonu.
Özellikler

*   **Abone Yönetimi:** Yeni abone kaydı, abone bilgileri güncelleme ve aktif/pasif durumu takibi.*
*   * **Veri Yönetimi (In-Memory):** Herhangi bir harici veritabanı (SQL/NoSQL) kurulumuna gerek duymadan, uygulama çalıştığı sürece verileri `List` ve `Map` yapıları üzerinde güvenle saklama.
* **Gelişmiş Terminal Arayüzü:** Tamamen konsol üzerinden yönetilen, kullanıcı dostu yönlendirme menüleri.

*   **Tarife ve Birim Fiyat Yönetimi:** Mesken (ev), ticarethane ve sanayi gibi farklı abone gruplarına göre dinamik birim fiyatlandırma.
*   **Otomatik Fatura Hesaplama:** İlk endeks ve son endeks bilgilerini alarak tüketim miktarını (kWh) bulma; vergi, fon ve bakım bedellerini otomatik ekleyerek toplam faturayı hesaplama.
*   Sistem, faturaları hesaplarken aşağıdaki standart formülü temel alır:

1.  **Tüketim Miktarı (kWh):** `Son Endeks - İlk Endeks`
2.  **Net Tüketim Bedeli:** `Tüketim Miktarı × Abone Grubu Birim Fiyatı`
3.  **Vergiler ve Fonlar:** Net bedel üzerine eklenen yasal kesintiler (KDV, Enerji Fonu vb.).
4.  **Toplam Tutar:** `Net Tüketim Bedeli + Vergiler + Dağıtım Bedeli*
6.   **Programlama Dili** | Java (JDK 11+) | İş mantığı ve hesaplama algoritmaları |
| **Veri Saklama** | Java Collections (`ArrayList`, `HashMap`) | Abone ve fatura kayıtlarının çalışma zamanında (Runtime) saklanması |
| **Kullanıcı Girdisi** | `java.util.Scanner` | Konsol üzerinden veri ve komut alımı |

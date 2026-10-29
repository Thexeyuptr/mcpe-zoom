# bey-zoom

QYCottage GDK ModLoader için yerel x64 Windows DLL dosyasıdır. Minecraft Bedrock GDK istemcisi için tasarlanmış olup `%APPDATA%\Minecraft Bedrock\mods` dizininden yüklenir.

## Kontroller

- Yakınlaştırmayı (zoom) etkinleştirmek için **C** tuşuna basılı tutun; tuşu bıraktığınızda normal görünüme dönersiniz.
- **C** tuşuna basılı tutarken fare tekerleğini kullanarak yakınlaştırma oranını **1x ile 20x** arasında, 0,5x'lik adımlarla ayarlayabilirsiniz.
- Yakınlaştırma için kullanılan fare tekerleği hareketleri "tüketilir" (işlenip başka bir yere iletilmez), bu sayede envanter çubuğundaki (hotbar) seçili öğe değişmez.

Mor renkli `bey-zoom` arayüz öğesi, Minecraft menü ekranlarında görünür; oyun dünyası kontrolü için fare imleci oyun tarafından yakalandığında (oyun içi modda) ise gizlenir. Yakınlaştırma özelliği yalnızca fare imlecinin oyun tarafından yakalandığı bu oynanış durumunda etkinleşir. Bu gösterge, kaynak paketlerinden (resource pack) bağımsızdır. DLL dosyası, karakter görünümü (skin) veya model dosyaları üzerinde herhangi bir değişiklik yapmaz. Yakınlaştırma işlemi, DWM (Desktop Window Manager) pencere kırpma yöntemiyle gerçekleştirilir; oyun dünyasının işleme mesafesini (render distance) artırmaz veya oyun içi kamera görüş açısını (FOV) değiştirmez. Daha yüksek yakınlaştırma oranları, mevcut ekran piksellerini büyütür; DWM küçük resim işlevleri, görüntü interpolasyon filtresi seçimine izin vermez.

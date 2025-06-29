## Kubernetes Dokümantasyon Projesi
Bu proje, Kubernetes ekosistemindeki temel kavramları, bileşenleri, yönetim araçlarını ve ileri düzey konuları kapsamlı ve detaylı bir şekilde açıklayan HTML belgelerinden oluşan bir koleksiyondur. Amacımız, Kubernetes öğrenme yolculuğunu kolaylaştırmak ve hem yeni başlayanlar hem de deneyimli kullanıcılar için güvenilir bir başvuru kaynağı sunmaktır.

Bu dokümantasyonun canlı bir versiyonuna [buradan](https://erelbi.github.io/k8s/) erişebilirsiniz.


## Proje Amacı ve Hazırlanma Nedeni
Modern yazılım geliştirme ve operasyon süreçlerinde, konteynerizasyon ve Kubernetes gibi platformlar vazgeçilmez hale gelmiştir. Ancak Kubernetes'in geniş ve karmaşık yapısı, öğrenme sürecini zorlaştırabilmektedir. Bu dokümantasyon projesi, aşağıdaki ihtiyaçları karşılamak üzere hazırlanmıştır:
* Kapsamlı Bilgi: Kubernetes'in temelinden ileri düzey konularına kadar geniş bir yelpazede bilgi sunmak.
Detaylı Açıklamalar: Her konuyu derinlemesine inceleyerek, sadece "ne" olduğunu değil, aynı zamanda "neden" ve "nasıl" çalıştığını da anlatmak.
* Görsel Destek: Karmaşık kavramları ve çalışma prensiplerini basitleştirmek için görseller ve diyagramlar kullanmak.
* Pratik Örnekler: Konuları pekiştirmek için ilgili YAML yapılandırmaları ve kullanım senaryoları sunmak.
* Erişim Kolaylığı: Tek sayfalık HTML belgeleri aracılığıyla konular arasında hızlı ve kolay geçiş imkanı sağlamak.
---
Bu projenin temel motivasyonu, Kubernetes öğrenimini daha erişilebilir, anlaşılır ve etkili hale getirmektir.
İçerik Yapısı
Proje, her biri belirli bir Kubernetes konusuna odaklanan ayrı HTML belgelerinden oluşmaktadır. Ana index.html sayfası, tüm bu belgelere kolayca erişim sağlayan bir navigasyon hub'ı görevi görür.
Mevcut belgeler ve kapsadıkları konular:
- index.html: Tüm dokümanlara bağlantı sağlayan ana sayfa.
- kubernetes-interactive-guide-tr.html: Kubernetes'e genel bir giriş, mimari ve temel kavramları interaktif bir şekilde açıklayan rehber.
- kubernetes-components-detail-tr.html: Kubernetes kontrol düzlemi ve çalışan düğüm (worker node) bileşenlerinin detaylı anlatımı.
- kubernetes-yaml-structures-detail-tr.html: ConfigMap, Secret, Deployment, PersistentVolumeClaim (PVC), Service ve NetworkPolicy gibi temel Kubernetes YAML yapılarının detaylı açıklamaları ve örnekleri.
- kubernetes-networkpolicy-detail-visual-tr.html: Kubernetes NetworkPolicy'nin detaylı anlatımı, çalışma prensipleri ve iptables ile eBPF gibi altta yatan teknolojilerin görsellerle açıklanması.
- kubernetes-cni-detail-visual-tr.html: Kubernetes CNI (Container Network Interface) kavramı, Calico ve Cilium gibi önde gelen CNI çözümlerinin detaylı karşılaştırması ve görselleri.
- kubernetes-dns-detail-tr.html: Kubernetes DNS çözümleri CoreDNS ve Node-Local-DNS'in detaylı anlatımı, çalışma prensipleri ve farkları.
- kubernetes-ci-cd-gitops-tools-tr.html: Kubernetes ortamında CI/CD ve GitOps için kullanılan GitLab Runner, GitLab Agent ve Flux CD araçlarının detaylı incelemesi.
- kubernetes-drain-cordon-detail-tr.html: Kubernetes'te düğüm bakımı ve iş yükü tahliyesi için kullanılan kubectl drain ve kubectl cordon komutlarının detaylı açıklaması.
- kubernetes-storage-detail-tr.html: Kubernetes'te kalıcı depolama yönetimi için PersistentVolume (PV), PersistentVolumeClaim (PVC) ve StorageClass kavramlarının detaylı anlatımı.
- kubernetes-job-cronjob-detail-tr.html: Tek seferlik ve zamanlanmış görevler için Kubernetes Job ve CronJob kaynaklarının detaylı açıklaması ve farkları.
- kubernetes-rbac-detail-tr.html: Kubernetes'te Rol Tabanlı Erişim Kontrolü (RBAC) mekanizmasının detaylı anlatımı ve örnekleri.
- kubernetes-hpa-vpa-detail-tr.html: Kubernetes'te otomatik yatay (HPA) ve dikey (VPA) Pod ölçeklendiricilerin detaylı açıklaması ve farkları.
- kubernetes-statefulset-daemonset-detail-tr.html: Kubernetes'te özel iş yükleri olan StatefulSet ve DaemonSet'in detaylı anlatımı ve farkları.
- kubernetes-ingress-detail-tr.html: Uygulamaları dış dünyaya açmak için Ingress ve Ingress Controller kavramlarının detaylı açıklaması.
- kubernetes-pdb-detail-tr.html: Pod Disruption Budget (PDB) ile gönüllü kesintiler sırasında uygulama kullanılabilirliğini sağlamanın detayları.
- kubernetes-talos-os-detail-tr.html: Kubernetes düğümleri için güvenli, minimal ve API odaklı işletim sistemi Talos OS'un detaylı anlatımı.

### Nasıl Kullanılır?
Projeyi Klonlayın: Bu depoyu yerel makinenize klonlayın.
git clone [depo-adresi]

```
Dosyaları Açın: Klonladığınız dizine gidin.
Tarayıcıda Açın: index.html dosyasını tercih ettiğiniz web tarayıcısında açın.
open index.html # macOS
start index.html # Windows
firefox index.html # Linux (veya tercih ettiğiniz tarayıcı)
```

Gezinin: Ana sayfadaki bağlantılar aracılığıyla farklı Kubernetes konularına dair detaylı belgelere erişebilirsiniz. Çoğu belgede, konu başlıklarına hızlı geçiş sağlayan gezinme menüleri ve dahili bağlantılar bulunmaktadır.

### Katkıda Bulunma

Bu projenin gelişimine katkıda bulunmak isteyen herkesi bekliyoruz! Hata düzeltmeleri, yeni konular, mevcut açıklamaları iyileştirme veya yeni görseller ekleme gibi her türlü katkı memnuniyetle karşılanır. Lütfen bir Pull Request (Çekme İsteği) oluşturarak veya bir sorun (Issue) bildirerek iletişime geçin.
### Lisans

Bu proje MIT Lisansı altında yayımlanmıştır. Bu lisans, yazılımın kullanımına, kopyalanmasına, değiştirilmesine, birleştirilmesine, yayımlanmasına, dağıtılmasına, alt lisanslanmasına ve/veya satılmasına izin verir. Daha fazla bilgi için lütfen MIT Lisansı metnine bakın.

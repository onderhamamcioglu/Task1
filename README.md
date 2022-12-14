# Proje 1
## Temel olarak bir platform üzerinde CI/CD tekniklerinin uygulanması

- [X] Seçilecek bir Continuous Integration platformunda (Azure DevOps, Gitlab, GitHub vb..) "Azure DevOps tercihimizdir" yeni proje
açıp, temel Work Item Management ihtiyaçları için örnek bir iki iş maddesi (PBI, Task vb..) oluşturmak.
- [Issues](https://github.com/onderhamamcioglu/Task1/issues?q=)
- [X] Örnek bir web projesinin kodlarını git üzerinden bu platforma yüklemek. (Mümkünse feature-branching tekniğini uygulamak)
- [Branches](https://github.com/onderhamamcioglu/Task1/branches)
- [X]  Pipeline tasarımı yapıp projenin her değişiklikle derlenmesinin ve paketlerin (artifact'larının) oluşmasının sağlanması
- [Pipeline](https://github.com/onderhamamcioglu/Task1/blob/prod/.github/workflows/pipeline.yml)
- [X]  Pipeline'a statik kod analizi yapan çözümlerin eklenmesi (SonarQube task'ının mümkünse QualityGateway'den geçmezse
pipeline'ın ilerlememesi)
- [Pipeline](https://github.com/onderhamamcioglu/Task1/blob/prod/.github/workflows/pipeline.yml) üzerinde [Super-Linter](https://github.com/github/super-linter) ile statik kod analizi gerçekleştiriliyor.
- [X] Temel test tekniklerinin otomasyon ile (pipeline üzerinde) uygulanması. Unit test'lerin çalışması, API testlerin koşturulması
(varsa bir iki adet yeterli.) "Postman tercihimizdir"
- [Pipeline](https://github.com/onderhamamcioglu/Task1/blob/prod/.github/workflows/pipeline.yml) üzerinde Newman ile Postman koleksiyonları çalıştırılıyor.
- [X] Fonksiyonel testlerin senaryolarının yazılıp, pipeline üzerinde entegrasyonun her hangi bir çözüm üzerinden yapılması.
(Selenium, Katalon, UFT vb..) "Opsiyonel"
- [Pipeline](https://github.com/onderhamamcioglu/Task1/blob/prod/.github/workflows/pipeline.yml) içerisine Java ile yazılmış [Selenium Testi](https://github.com/onderhamamcioglu/Task1/tree/prod/SeleniumTest) eklendi
- [X] Oluşan ve testlerden geçmiş paketlerin otomatik olarak bir ortama (Local sunucu, VM veya bulut ortamında olabilir)
teslimatının "deployment" yapılması
- ![Pipeline](https://github.com/onderhamamcioglu/Task1/actions/workflows/pipeline.yml/badge.svg) | https://task1-fqoaam3z4q-ey.a.run.app/
